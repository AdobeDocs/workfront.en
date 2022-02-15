---
filename: reset-user-password-eauth
product-area: user-management
navigation-topic: manage-your-workfront-account
---



# Reset a user's password with Enhanced Authentication {#reset-a-users-password-with-enhanced-authentication}

When Enhanced Authentication (eAuth) is enabled for your Workfront Environment, a *`Workfront administrator`* can’t reset login credentials for another user. This differs from Workfront environments without eAuth or those environments for which Single Sign On (SSO) is enabled.


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



## Reset a user’s password in an eAuth enabled environment {#reset-a-user-s-password-in-an-eauth-enabled-environment}




1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">Main Menu icon</span> and select  <span class="bold">Users</span>.</MadCap:conditionalText>`
1.  ![](assets/main-menu-users-highlighted-nwe-350x456.png)

1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Select the  <span class="bold">User</span> that requires a password reset.</MadCap:conditionalText>`
1.  ![](assets/100520classicnweselectuser-350x105.png)

1. Click the `More button` that appears after you've chosen the desired `User` and select the `Send Forgot Password Email` option from the drop-down menu.

1.  ![](assets/100520classicnwesendemail-350x134.png)



After selecting the `Send Forgot Password Email` option, an email is sent to the selected user that contains instructions for them to change their own password.


![](assets/pwresetemail-resized-350x461.png)


