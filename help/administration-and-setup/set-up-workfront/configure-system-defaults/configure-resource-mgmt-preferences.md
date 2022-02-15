---
filename: configure-resource-mgmt-preferences
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
---



# Configure Resource Management preferences {#configure-resource-management-preferences}

As an *`Adobe Workfront administrator`* you can configure the Resource Management Preferences for your system. 


The Resource Management preferences determine how user availability and FTE are calculated for the *`Workfront`* resource scheduling and planning tools.


For information about planning and scheduling resources in *`Workfront`*, see [Get started with Resource Management](get-started-resource-management.md).


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



## Configure Resource Management preferences {#configure-resource-management-preferences-1}



>[!NOTE]
>
>Because this is a global setting, this selection affects all the calculations for the entire system, for all users, in all the resource management tools, and for all Resource Pools.





1.  Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).
1.  Click `Resource Management`. 
1.  Select one of the following methods to calculate the availability of users in *`Workfront`*: 
    
    
    * `The Default Schedule`: *`Workfront`* uses the Default Schedule of the system and the individual FTE of the user to calculate the Available Hours of the user in resource management tools.   
      For more information about schedules, see [Create a schedule](create-schedules.md)For more information about the value of the user FTE, see&nbsp; [Edit a user's profile](edit-a-users-profile.md)  
      The Available Hours for the user are calculated by this formula:  
    
    
      ```    
      User Available Hours = Default Schedule Hours * User FTE value
      ```    
    
  
      For example, if the Default Schedule is 40 hours a week and the FTE in the profile of the user is 0.5, the user is available to work for 20 hours a week.  
    
    * `The User's Schedule`: *`Workfront`* uses the Default Schedule of the system and the schedule of the user to calculate the Available FTE value of the user in resource management tools. The value of the FTE of the user is ignored. This is the default setting.  
      The Available FTE for the user is calculated by this formula:  
    
    
      ```    
      User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours
      ```    
    
  
      For example, if the Default Schedule is 40 hours a week and the schedule of the user is 30 hours a week,&nbsp;the FTE of the user is 0.75.&nbsp;
    
    
      >[!NOTE]
      >
      >If the user is not associated with a schedule, the Available Hours for the user are calculated using the Default Schedule.
    
    
    
    
    

1.  Click `Save`.  



