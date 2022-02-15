---
filename: config-time-logged-hrs-days
product-area: timesheets;setup
navigation-topic: configure-timesheet-preferences
---



# Configure whether time is logged in hours or days {#configure-whether-time-is-logged-in-hours-or-days}

As a user with a Planner license, you can configure whether you log time in *`Adobe Workfront`* in hours or days. System administrators can configure this setting for individual users or for multiple users in their organization. By default, users log time in hours. For information about how to log time in *`Workfront`*, see [Log time](log-time.md).


>[!NOTE]
>
>We recommend logging time in the same way, either hours or days, across the organization to ensure reporting accuracy.




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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Planners can configure time for themselves. Only a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can configure time for other users.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.



1. Do either of the following, depending on your objective and your access level in the system: 
    
    
    * `Planner user configuring time logging for yourself:` `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the Main Menu icon. Click your user avatar, then click the  <span class="bold">More</span> icon next to your name and select  <span class="bold">Edit</span>.</MadCap:conditionalText>`
    
    * `System administrator configuring time logging for others:` Begin editing one or more user accounts, as described in [Edit a user's profile](edit-a-users-profile.md).
    
    
    
1.  In the resulting dialog box, in the `Resource Planning` section, locate the `Log Time in` option.


   ![](assets/new-timesheet-log-hours-350x249.png)



1. (Conditional) If you are a system administrator editing multiple users simultaneously, select `Log Time in`.
1. Select from the following options for logging time:   


1.  (Conditional) If you selected to log time in days, in the `Equivalent Hours for Full Workday` field, type the number of hours that equal a full day. One day on a user's timesheet is the equivalent of the number of hours you enter here.


   Consider the following when configuring this setting: 

    
    
    * This option is not available when configuring to log time in hours.
    * This option is used only for the purpose of logging time. This option is not related to the `Schedule` option that is also available when editing a user. The `Schedule` option is used when calculating timelines and in other areas of *`Workfront`*. (For more information about using the `Schedule` option, see [Create a schedule](create-schedules.md).)&nbsp;
    
    
    

1. Click `Save Changes`.


