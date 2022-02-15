---
filename: error-message-on-mobile-app
content-type: tips-tricks-troubleshooting
product: mobile
navigation-topic: tips-tricks-and-troubleshooting-mobile-apps
---



# Error Message on the *`Adobe Workfront`* Mobile App: "Your account is not API enabled." {#error-message-on-the-adobe-workfront-mobile-app-your-account-is-not-api-enabled}



## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p> Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Plan</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>System administrator </p> </td> 
  </tr> 
 </tbody> 
</table>



## Problem {#problem}

When trying to log in to the *`Adobe Workfront`* mobile app, you receive the following error: *Your account is not API enabled. Let your system admin know and they'll get you set up. Sorry about that.*


## Cause {#cause}

Your *`Workfront administrator`* has not enabled your *`Workfront`* environment to be accessed from a mobile device.


## Solution {#solution}




1. Log into the *`Workfront`* web application as a *`Workfront`* Administrator.

1. Go to the `Setup` area.
1. Expand the `System` menu, then click `Preferences`.

1. Under the `Security` section, select the `Let people use *`Workfront`*'s mobile applications and the *`Workfront`* Outlook Add-In`&nbsp;option to enable it.&nbsp;

1. Click `Save`.  
   All users in the system can now access *`Workfront`* from their mobile apps, and from Outlook.



