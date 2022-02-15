---
filename: configure-basic-info
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
---




# Configure basic info for your system {#configure-basic-info-for-your-system}

As part of configuring your `Workfront` system, you can manage details about your organization in the Basic Info section of your Customer Info page.&nbsp;


## Access Customer Info {#access-customer-info}

The customer represents the `Workfront` instance for your organization. The options in this area are unique to you, as a customer of `Workfront`.


To access the Customer Info page:



1. <![CDATA[]]>Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of `Workfront`, then click **Setup** ![](assets/setup-gear-icon.png).  

1.  In the left panel, click **System** > **Customer Info**. 


   Depending on the `Workfront` plan that you have purchased, some sections might be missing from the Customer Info page. Contact your Account Representative if you need to find out which `Workfront` plan your organization uses.


   The sections available in the Customer Info area are:

    
    
    * **Basic Info**   
      For information about configuring basic information in `Workfront`, see [Configure Basic Info](#configuring-basic-info).
    
    *  **API Key Settings** 
    *  **IP Whitelist** 
    * **License**   
      For information about licenses, see [Manage available licenses in your system](manage-available-licenses-in-your-system.html.md).
    
    
    





## Configure Basic Info {#configure-basic-info}

Inside the Basic Info area of your Customer Info page, some details about your customer are configured by `Workfront` and they display in a read-only mode. Other details can be configured by you. Any options you can edit in this area have a global effect on all users in `Workfront`.


To&nbsp;configure your Basic Info section in your Customer Info area:



1. <![CDATA[]]>Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of `Workfront`, then click **Setup** ![](assets/setup-gear-icon.png).<![CDATA[]]>

1. In the left panel, click **System** > **Customer Info**. 

1.  In the **Basic Info** section at the top of the **Customer Info** page, find the following information about your instance with `Workfront`:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" style="width: 244px;"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Name</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">The name of your organization, which also matches the name of your company. This is added&nbsp;by <span class="WFVariablesProdNameWF">Workfront</span> and it cannot be edited.<br></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray"><b>Cluster Setup</b> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">The cluster number for your instance. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray"><a name="Admin_Email"></a>Admin Email</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>The email address of your&nbsp;<span class="WFVariablesAdminWF">Workfront administrator</span>. You can edit this field to match the email address of one of your <span class="WFVariablesAdminWF-plur">Workfront administrators</span>. The user associated with this email address is considered the main <span class="WFVariablesAdminWF">Workfront administrator</span> of your <span class="WFVariablesProdNameWF">Workfront</span> system. Any site-wide communication from <span class="WFVariablesProdNameWF">Workfront</span> is directed&nbsp;to this email address, so it is important to keep it updated.</p> <p>Note:  You cannot deactivate, delete, or change the Access Level of the user associated with the Admin Email.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Domain</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>The domain is set by <span class="WFVariablesProdNameWF">Workfront</span> when your account is created.</p> <p>The domain identifies your&nbsp;unique sub-domain of the URL you use to access <span class="WFVariablesProdNameWF">Workfront</span>.<br>For example, if your organization has been assigned the domain "mycompany," the URL you use to access <span class="WFVariablesProdNameWF">Workfront</span> is&nbsp;<i>https://mycompany.my.workfront.com</i>.<br>You cannot edit the domain yourself. If you want to change your domain, you can contact <span class="WFVariablesProdNameWF">Workfront</span> Customer Support. For more information about&nbsp;contacting <span class="WFVariablesProdNameWF">Workfront</span>&nbsp;Customer Support, see <a href="contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Time Zone</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>This is the default time zone of your <span class="WFVariablesProdNameWF">Workfront</span> instance. You can edit this field to match the time zone of your primary <span class="WFVariablesProdNameWF">Workfront</span> location. The time zone you select affects the following: </p> 
    <ul> 
     <li value="1">Controls the date and time displayed in outgoing emails. </li> 
     <li value="2">It is selected as the default time zone for new users when they are created.</li> 
    </ul> <p>Users can modify&nbsp;the&nbsp;time zone for their <span class="WFVariablesProdNameWF">Workfront</span>&nbsp;instance under their profile. When&nbsp;users modify their time zone, the date and time in their emails from <span class="WFVariablesProdNameWF">Workfront</span> match their profile preferences. For more information about modifying user profile&nbsp;preferences, see&nbsp;<a href="configure-my-settings.md" class="MCXref xref">Configure My Settings</a>It is selected as&nbsp;the default time zone when you create a new schedule. For more information about creating schedules, see <a href="create-schedules.md" class="MCXref xref">Create schedules</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Locale</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Controls the language, date, and number format used in outgoing email messages. The locale selected here&nbsp;is&nbsp;the default when new users are created. Users can modify their locale, in their user profile. When&nbsp;users modify their locale, the language, date and number format in their emails from <span class="WFVariablesProdNameWF">Workfront</span> match their profile preferences. For more information about modifying your profile preferences, see <a href="configure-my-settings.md" class="MCXref xref">Configure My Settings</a>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Storage Quota</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>This is the amount of document storage space available in&nbsp;your <span class="WFVariablesProdNameWF">Workfront</span> instance.<br>The quota contains documents that you upload directly to <span class="WFVariablesProdNameWF">Workfront</span>.<br>It does not include:</p> 
    <ul> 
     <li value="1">Documents you link to&nbsp;<span class="WFVariablesProdNameWF">Workfront</span> from any other third-party service provider (SharePoint, Google Drive, Webdam, Box, Dropbox, any other Document Asset Management provider).</li> 
     <li value="2">Your <span class="WFVariablesProdNameWF">Workfront</span> data (projects, tasks, issues, users, and so forth).</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray">Product Version</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">This is the type of <span class="WFVariablesProdNameWF">Workfront</span> instance that is assigned to you. The product version for most <span class="WFVariablesProdNameWF">Workfront</span> customers is <b>Enterprise</b>.</td> 
  </tr> 
 </tbody> 
</table>


1. Click **Save**.


