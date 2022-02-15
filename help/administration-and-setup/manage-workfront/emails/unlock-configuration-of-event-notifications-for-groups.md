---
filename: unlock-configuration-of-event-notifications-for-groups
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
---



# Unlock or re-lock configuration of event notifications for groups {#unlock-or-re-lock-configuration-of-event-notifications-for-groups}

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.


If you are an *`Adobe Workfront administrator`*, you can unlock or re-lock the ability for *`group administrators`* to configure an event notification for top-level groups they manage. Configuration of an event notification consists of activating or deactivating it.


If there are any groups above the group you manage, their administrators can also do this for your group. The same is true for *`Workfront administrators`* (for any group).


When an administrator configures an event notification for a group, the configuration affects users for whom that group, or one of its subgroups, is their Home Group. In their user profiles, these users see the event notifications that are activated for their Home Group instead of the event notifications that are activated system-wide. For more information, see [View and configure event notifications for a group](view-and-configure-event-notifications-group.md).


>[!NOTE]
>
>
>
>
>* A *`Workfront administrator`* can unlock and re-lock configuration for an event notification in both *`Adobe Workfront Classic`* and *`the new Adobe Workfront experience`*. But a *`group administrator`* can configure that event notification for a group only in *`the new Adobe Workfront experience`*. *`Group administrators`* using *`Adobe Workfront Classic`* can switch to *`the new Adobe Workfront experience`* to configure unlocked event notifications for a group, then switch back to *`Adobe Workfront Classic`* to see the changes in effect.
>
>* Subgroups inherit group-level event notification configurations from the top-level groups above them.
>
>





## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Plan</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>System administrator</p> </td> 
  </tr> 
 </tbody> 
</table>



## Unlock or re-lock the ability to configure an event notification {#unlock-or-re-lock-the-ability-to-configure-an-event-notification}



>[!IMPORTANT] {type="important"}
>
>When you re-lock a notification, all groups in the system inherit the notification exactly as you set it. This overrides any changes that *`group administrators`* might have made for their groups, so it’s a good idea to consult with them first.





1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. Click `Email` > `Notifications`.

1.  Make sure the `Event Notifications` tab is open.
1.  Click the icon to the right of the notification ![](assets/lock-toggle-button.png) to switch it to the unlocked position ![](assets/unlock-toggle-button.png) (or do the opposite to re-lock an unlocked notification).

   Or


   If you want to unlock or re-lock multiple notifications all at once, select them, then click the Unlock ![](assets/unlock-icon-toolbar.png) or Lock ![](assets/lock-icon-locked-qs.png) button that displays in the toolbar above the list.

1. Click `Save`.
1. (Optional) If you want to configure the event notification for a top-level group instead of leaving this task to the group’s administrator, you can do one of the following:
    
    
    * Delete `System Event Notifications` in the search box above the list of notifications, search for and select the name of the top-level group to list its notifications, then activate or inactivate the unlocked notifications in the list that displays.
    * Click `Groups` in the left menu, then click the name of the top-level group. Click `Event Notifications` in the left panel, then configure the unlocked event notification, as explained in [View and configure event notifications for a group](view-and-configure-event-notifications-group.md).
    
    
    


