---
filename: lock-or-unlock-a-group-timesheet-hour-preference
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
---



# Lock or unlock a group timesheet and hour preference {#lock-or-unlock-a-group-timesheet-and-hour-preference}

If you are a *`group administrator`*, you can configure and then lock a timesheet and hour preference for your group after a *`Workfront administrator`* unlocks it at the system level.


Locking a preference`<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">  at the group level</MadCap:conditionalText>` ensures that everyone`<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">  in your group and in its subgroups</MadCap:conditionalText>` is using the same setting for that preference. Though you can still reconfigure a preference that you lock, *`group administrators`* can’t do so for `<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups"> lower subgroups</MadCap:conditionalText>`.


Conversely, unlocking a preference`<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">  at the group level</MadCap:conditionalText>` allows `<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups"> sub</MadCap:conditionalText>` *`group administrators`* more flexibility to manage the way their groups work with those items. When a `<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups"> group </MadCap:conditionalText>`preference is unlocked, *`group administrators`*`<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">  of lower subgroups</MadCap:conditionalText>` can reconfigure it for `<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups"> those subgroups</MadCap:conditionalText>`.


This is parallel to the ability that a *`Workfront administrator`* has to lock or unlock a preference for everyone in the system.


For information about how a *`Workfront administrator`* can lock or unlock a timesheet and hour preference for all groups in the system, see [Configure timesheet and hour preferences](timesheet-and-hour-preferences.md).


For information about configuring a timesheet and hour preference for a group, see [Configure timesheet and hour preferences for a group](configure-timesheet-hour-preferences-group.md).


>[!NOTE]
>
>
>
>
>*  Configuring an unlocked preference for a group doesn’t affect that preference for any subgroups below the group.
>
>
>  However, when a new subgroup is created, it inherits the preference settings and locked or unlocked state of the group immediately above it.
>
>*  If you move a group under a group that has a locked preference, the moved group inherits that preference and it is locked for the moved group. 
>*  If you move a group under a group that has an unlocked preference, the moved group is not affected by that preference.
>
>
>  If the preference in the moved group is locked at the time of the move, it remains locked, but the *`group administrator`* can unlock it now because it is unlocked for the parent group.
>
>
>





## Access requirements {#access-requirements}

You must have the following to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> <p>You must be a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> of the group or a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For more information, see <a href="group-administrators.md" class="MCXref xref">Group administrators</a> and <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your *`Workfront administrator`*.


## Lock or unlock a group timesheet and hour preference {#lock-or-unlock-a-group-timesheet-and-hour-preference-1}



>[!TIP] {type="tip"}
>
>If you are a *`Workfront administrator`*, you can bypass steps 1-4 by going to Setup > Timesheet &&nbsp;Hours > Preferences, then searching for the group’s name in the box at the top of the page.





1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. In the left panel, click `Groups`.
1. Click the name of the group where you want to lock or unlock a timesheets and hours preference.
1. In the left panel, click `Timesheets and Hour` `s Preferences`.

1.  On the page that appears, do any of the following:

    
    
    *  If you want administrators of groups below your group to be able to configure a preference for their groups, unlock it ![](assets/unlock-toggle-button.png).
    *  If you want all groups below yours to use your configuration for a preference, make sure that it is locked ![](assets/lock-toggle-button.png) (this is the default).
    
    
      >[!IMPORTANT] {type="important"}
      >
      >It's important to communicate with the administrators and users in groups below yours to ensure that all needs are accounted for in the way you configure a locked preference. When you lock it, your configuration for it is inherited by any subgroups below. And if the preference has been unlocked for any period of time, your configuration replaces those that *`group administrators`* in lower subgroups might have made.
    
    
    
    
    

1. Click `Save`.


