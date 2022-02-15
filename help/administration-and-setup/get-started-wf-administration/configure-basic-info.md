---
filename: configure-basic-info
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
---



# Configure basic information for your system {#configure-basic-information-for-your-system}

As part of configuring your *`Adobe Workfront`* system, you can manage details about your organization in the Basic Info section of your Customer Info page.


## Access requirements {#access-requirements}

You must have the following to perform the steps in this article:

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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>You must be a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For more information, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Access Customer Info {#access-customer-info}

The customer represents the *`Workfront`* instance for your organization. The options in this area are unique to you, as a customer of *`Workfront`*.


To access the Customer Info page:



1. <![CDATA[]]>Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).  

1.  In the left panel, click `System` > `Customer Info`. 


   Depending on the *`Workfront`* plan that you have purchased, some sections might be missing from the Customer Info page. Contact your Account Representative if you need to find out which *`Workfront`* plan your organization uses.


   The sections available in the Customer Info area are:

    
    
    *  `Basic Info` 
    
    
      For information about configuring basic information in *`Workfront`*, see [Configure Basic Info](#configuring-basic-info).
    
    *  `API Key Settings` 
    
    
      For information about API key settings, see [Manage API keys](manage-api-keys.md).
    
    *  `IP Allowlist` 
    
    
      For information about adding the IP addresses to your allowlist for where your users can access *`Workfront`*, see [Configure your firewall](configure-your-firewall.md).
    
    *  `License` 
    
    
      For information about licenses, see [Manage available licenses in your system](manage-available-licenses-in-your-system.md).
    
    
    





## Configure Basic Info {#configure-basic-info}

Inside the Basic Info area of your Customer Info page, some details about your customer are configured by *`Workfront`* and they display in a read-only mode. Other details can be configured by you. Any options you can edit in this area have a global effect on all users in *`Workfront`*.


To&nbsp;configure your Basic Info section in your Customer Info area:



1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. In the left panel, click `System` > `Customer Info`. 

1.  In the `Basic Info` section at the top of the `Customer Info` page, find the following information about your instance with *`Workfront`*:

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" style="width: 244px;"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Name</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">The name of your organization, which also matches the name of your company. This is added by <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> and it cannot be edited.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Cluster Setup </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">The cluster number for your instance.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><a name="Admin_Email"></a>Admin Email</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>The email address of your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. You can edit this field to match the email address of one of your <span class="mc-variable WFVariables.AdminWF-plur variable varname">Workfront administrators</span>. The user associated with this email address is considered the main <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> of your <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> system. Any site-wide communication from <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> is directed&nbsp;to this email address, so it is important to keep it updated.</p> <p>Note:  You cannot deactivate, delete, or change the Access Level of the user associated with the Admin Email.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Domain</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>The domain is set by <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> when your account is created.</p> <p>The domain identifies your&nbsp;unique sub-domain of the URL you use to access <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>.<br>For example, if your organization has been assigned the domain "mycompany," the URL you use to access <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> is <i>https://mycompany.my.workfront.com</i>.<br>You cannot edit the domain yourself. If you want to change your domain, you can contact <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> Customer Support. For more information about&nbsp;contacting <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>&nbsp;Customer Support, see <a href="contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Time Zone</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>This is the default time zone of your <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> instance. You can edit this field to match the time zone of your primary <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> location. The time zone you select affects the following: </p> 
    <ul> 
     <li>Controls the date and time displayed in outgoing emails. </li> 
     <li>It is selected as the default time zone for new users when they are created.</li> 
    </ul> <p>Users can modify the time zone for their <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>&nbsp;instance under their profile. When&nbsp;users modify their time zone, the date and time in their emails from <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> match their profile preferences. For more information about modifying user profile&nbsp;preferences, see <a href="configure-my-settings.md" class="MCXref xref">Configure My Settings</a>. It is selected as&nbsp;the default time zone when you create a new schedule. For more information about creating schedules, see <a href="create-schedules.md" class="MCXref xref">Create a schedule</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Locale</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Controls the language, date, and number format used in outgoing email messages. The locale selected here&nbsp;is&nbsp;the default when new users are created. Users can modify their locale, in their user profile. When users modify their locale, the language, date and number format in their emails from <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> match their profile preferences. For more information about modifying your profile preferences, see <a href="configure-my-settings.md" class="MCXref xref">Configure My Settings</a>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Storage Quota</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>This is the amount of document storage space available in&nbsp;your <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> instance.<br>The quota contains documents that you upload directly to <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>.<br>It does not include:</p> 
    <ul> 
     <li>Documents you link to&nbsp;<span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> from any other third-party service provider (SharePoint, Google Drive, Webdam, Box, Dropbox, any other Document Asset Management provider).</li> 
     <li>Your <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> data (projects, tasks, issues, users, and so forth).</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Product Version</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">This is the type of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> instance that is assigned to you. The product version for most <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> customers is <span class="bold">Enterprise</span>.</td> 
  </tr> 
 </tbody> 
</table>


1. Click `Save`.


