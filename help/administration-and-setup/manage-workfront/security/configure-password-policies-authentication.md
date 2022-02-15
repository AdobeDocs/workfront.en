---
filename: configure-password-policies-authentication
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
---



# Configure password policies for authentication {#configure-password-policies-for-authentication}



>[!IMPORTANT] {type="important"}
>
>The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Business Platform.
>
>
>If your organization has been onboarded to the Adobe Business Platform, authentication is handled automatically as part of that integration. You do not need to configure or enable this functionality.
>
>
>For a list of procedures that differ based on whether your organization is migrated to Adobe IMS, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](actions-in-admin-console.md).



As an *`Adobe Workfront administrator`*, you can configure password policy options to customize the authentication experience to your *`Workfront`* system.


We recommend that you configure authentication preferences during the *`Workfront`* implementation and only occasionally revisit them afterward.


Improved password management capabilities are coming soon or might already be available for your organization. Use either of the following sections, depending on whether your organization has access to the new authentication experience.


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



## Configure authentication (available for all customers) {#configure-authentication-available-for-all-customers}

Authentication options are displayed for all customers.&nbsp;Improved password management capabilities are coming soon or might already be available for your organization, as described in the&nbsp;section&nbsp; [Configure enhanced authentication (coming soon)](#configuring-unified-authentication) in this article.


To configure authentication preferences:



1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. Click `System` > `Authentication`.

1.  Select any of the following fields to establish the authentication settings for your&nbsp;organization:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Force users to reset their password every <em>&lt;value&gt;</em> days</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">This establishes the time frame for users to reset their <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> password. By default, this option is disabled. When you enable it, you can choose between 30, 60, 90, 120, 180 days. The default is 30 days.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Don't allow users to set the same password as any of their previous&nbsp;<em>&lt;value&gt;</em> passwords</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>This field prohibits users from reusing passwords for a set number of resets. By default, this field is disabled. When you enable it, you&nbsp;can set this value to 5, 10, or 15 resets before a password can be reused.</p> <p>When this option is selected, users cannot reset their passwords more than one time in a given day</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">If an incorrect password is entered five consecutive times, lock the account for&nbsp;<em>&lt;value&gt;</em> minutes:&nbsp;</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Select&nbsp;how long a user will be locked out of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> after entering an incorrect password five consecutive times. By default, this option is enabled, and the amount of wait time is 10 minutes. You can lock accounts for 10 minutes, 30 minutes, 1 hour, 8 hours, or 24 hours. </p> <p>Manually resetting the password for the user overrides this default wait value. <br>Users can reset their own passwords when they are locked out via the login screen. For more information about how they can reset their password, if they forgot it, see <a href="reset-your-password.md" class="MCXref xref">Reset your password</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Passwords must contain at least&nbsp;<em>&lt;value&gt;</em> different types of characters:</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Determines how strong user passwords are required to be by allowing you to select the number of different types of characters required in your passwords.</p> <p>A recognizable dictionary word cannot&nbsp;be used as a password.<br>By default,&nbsp;<span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> requires that at least 2&nbsp;of the following are present in passwords (you can also require&nbsp;3 of these characters to be present for a valid password): </p> 
    <ul> 
     <li>Uppercase characters</li> 
     <li>Lowercase characters</li> 
     <li>Numbers</li> 
     <li>Symbols</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>


1. Click `Save`.




## Configure enhanced authentication (coming soon) {#configure-enhanced-authentication-coming-soon}

This section describes the enhanced authentication experience, which might not yet be available for your organization. If your organization has not been migrated to the new authentication experience, you must configure the authentication settings, as described in [Configure authentication (available for all customers)](#configuring-legacy-authentication).


To configure enhanced authentication preferences:



1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1.  Click `System` > `Enhanced` `Authentication`.
1.  In the `Password Length`&nbsp;box, enter the minimum number of characters&nbsp;required for a valid password.


   *`Workfront`* requires at least 6 characters.

1.  (Optional) In the  `Password Requirements`section, select the&nbsp;types of characters required in user passwords.


   You can increase the strength of user passwords by requiring any or all the types of characters in the Password Requirement section. The following options are available:


1. Click `Save`.


