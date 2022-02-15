---
filename: username-already-in-use
content-type: tips-tricks-troubleshooting
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-groups
---



# Username Already in Use {#username-already-in-use}



## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
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



## Question {#question}

When creating a new user, a Whoops error is displayed stating that the username is already taken. There are no other occurrences of this email in the system. Why is this being displayed?


## Solution {#solution}

This can occur either because the username or email address is not unique in the current *`Adobe Workfront`* instance. Users can have the same username or email address in separate instances. For example, User A could have the following email addresses associated with a Workfront account: usera@company1.com and usera@company2.com.


>[!NOTE]
>
>The primary Workfront administrator can't have the same username or email address if they are in separate Workfront instances on the same cluster.   
  
>If the instances are on different clusters, the primary admin can have the same username or email address. You can view the cluster your instance is on under Setup > System > Customer Info.




### Check if your username is unique in your instance {#check-if-your-username-is-unique-in-your-instance}

Ensure that the username and email address is unique in the current *`Workfront`* instance:



1. As the *`Workfront administrator`*, go to the `People` tab, then click the `People` subtab.

1. In the list of people, look in the `Email` column to ensure there are no duplicate emails.
1. Add a column for username to the view. 
    
    
    1. In the `View` drop-down menu, click  `Customize View`.
    
    1. Click  `Add Column`.
    1. In the search field, type *username*.
    1. Select `User` > `Username`.
    
    1. Save the view.  
       This results&nbsp;in a view to display the usernames where you can look for the duplicate.
    
    
1. In the list of people, look in the `Username` column to ensure there are no duplicate usernames.


