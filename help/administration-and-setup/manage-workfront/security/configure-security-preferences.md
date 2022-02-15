---
filename: configure-security-preferences
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
---



# Configure system security preferences {#configure-system-security-preferences}



>[!IMPORTANT] {type="important"}
>
>The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Business Platform.
>
>
>If your organization has been onboarded to the Adobe Business Platform, authentication is handled automatically as part of that integration. You do not need to configure or enable this functionality.
>
>
>For a list of procedures that differ based on whether your organization is migrated to Adobe IMS, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](actions-in-admin-console.md).



As an *`Adobe Workfront administrator`*, you can configure security preferences for your *`Workfront`* system:



* Access to *`Workfront`* from mobile apps and other integrated applications
* Rules for embedding *`Workfront`* in an iframe


Changes that you make in the system preferences impact all users in your system, and their experience in *`Workfront`*.


We recommend that you configure your system security preferences during the *`Workfront`* implementation and only occasionally revisit them after that.


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



## Configure your system security preferences {#configure-your-system-security-preferences}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. In the left panel, click `System` > `Preferences`.  

1.  In the `Security` section, select any of the following fields to establish the security settings for your organization:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <p>Allow embedding of <span class="bold">Workfront</span> in an iframe</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Lets you embed <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> in an iframe.<p>This option is disabled by default.</p><p>Important: Displaying a web-based application in an iframe makes the application susceptible to a click-jacking security vulnerability.</p></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Allow SAML 2.0 authentication in Office 365 add-ins</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Lets you embed <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> in an iframe only for Office 365 add-ins when <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> is integrated with a SAML 2.0 single sign-on solution. </p> <p>This option is enabled by default.</p> <p>Note:  If you enable the option above, <span class="bold">Allow embedding of Workfront in an iframe</span>, the option <span class="bold">Allow SAML 2.0 authentication in Office 365 add-ins</span> is enabled and dimmed.<br></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Enable the use of session information when creating External Page URLs</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Allows users to use the Session ID information of a site when adding an External Page to a Dashboard.<br></p> <p>For more information about adding External Pages to a Dashboard, see <a href="embed-external-web-page-dashboard.md" class="MCXref xref">Embed an external web page in a dashboard</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Let people use Workfront's mobile applications and the <span class="bold">Workfront</span> Outlook Add-In</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Allows users to access the mobile apps (<span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> View for iPad and mobile phone apps) and the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> Outlook app.</p> <p>This option is enabled by default. </p> <p>For information about <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> View, see <a href="_use-workfront-view.md" class="MCXref xref">Use Adobe Workfront View</a>. For more information about the mobile apps, see <a href="use-the-mobile-app.md" class="MCXref xref">Use the Adobe Workfront mobile app</a>.</p> <p>For more information about the Outlook plugin, see <a href="set-up-workfront-for-outlook.md" class="MCXref xref">Set up Adobe Workfront for Outlook</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <p>Collaborate with people without Workfront accounts by using email addresses</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Allows <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> users to share certain items with people without a <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> account by including their email address instead of their name. Users can share the following items with external users by using their email address:
    <ul>
     <li>Document<br></li>
     <li>Document request<br></li>
     <li>Document approval</li>
     <li>Calendar</li>
    </ul><p>This option is enabled by default.</p></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Require external users to register with a password</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Requires external users to register before they are able to view items in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>. By default, this option is disabled. When you enable this option, people without a <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> account who are included in certain updates by their email address, will be prompted to create an account before they can view the item they are included on. This creates an External User account for them.</p> <p>This option is disabled by default.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Automatically log users out after</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Note: This is not currently available. We are working on authentication enhancements that will allow you to log out inactive users automatically after a period of time that you choose.</p> <p>Lets you specify when a user is logged out of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, after a period of inactivity. By default, users are logged out after 8 hours of inactivity. </p> <p>This option also affects <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> customers who are using a single sign-on solution.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Automatically log mobile users out after </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Lets you specify when a user is logged out of the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> application, after a period of inactivity. By default, users are logged out after 7 days of inactivity. <p>This option also affects <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> customers who are using a single sign-on solution.</p></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader"><span class="bold">Enable Zoom integration in the updates stream</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Lets you enable or disable the Zoom integration in the Updates area for all users in the organization.<br>The Zoom integration allows users to add a Zoom meeting URL to a comment or reply in the Updates area. For more information, see <a href="https://one.workfront.com/s/article/Using-the-Zoom-integration?language=en_US">Using the Zoom integration</a>. Also see the section <a href="update-work.md#add" class="MCXref xref">Add an update to a work item</a> in the article<a href="update-work.md" class="MCXref xref">Update work</a>.</p> <p>Users can uninstall the Zoom integration in their personal instance of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>. For more information, see <a href="https://one.workfront.com/s/article/Uninstalling-the-Zoom-integration?language=en_US">Uninstalling the Zoom integration</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>


1.  Click `Save`.


   The changes that you saved here affect the experience of all the users in *`Workfront`* and anyone who interacts with them as an external user.



