---
filename: disable-document-integrations
title: Disable document integrations
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
---



# Disable document integrations {#disable-document-integrations}

As an *`Adobe Workfront administrator`*, you can disable the connection between *`Workfront`* and any of the third-party document providers.&nbsp;


When you disable the connection between *`Workfront`* and a document provider, the links to the documents disappear from *`Workfront`*. Users can no longer see the linked documents, they cannot make any changes to the documents through the *`Workfront`* links, and they cannot add more documents to that provider.&nbsp;



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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>You must be a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For information on <span class="mc-variable WFVariables.AdminWF-plur variable varname">Workfront administrators</span>, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Disable cloud provider integrations {#disable-cloud-provider-integrations}

To disable document integrations for *`Workfront DAM`*, Workfront Library, Box, Dropbox, Google Drive, Microsoft&nbsp;OneDrive, WebDAM:



1. Log in to *`Workfront`* as a *`Workfront administrator`*.

1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. Click `Documents` > `Cloud Providers`.

1. Deselect any of the cloud providers you want to disconnect from *`Workfront`*.
1.  Click `Save`.


   Users are not able to connect to the specific cloud provider you disabled, and they can no longer link documents from that cloud provider to *`Workfront`*.





## Disable the SharePoint integration {#disable-the-sharepoint-integration}




1. Log in to *`Workfront`* as a *`Workfront administrator`*.

1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1.  Expand `Documents`, then click `SharePoint Integration`.
1.  Select the SharePoint integration you want to disable.
1. Click `Disable`.  
   Users are not able to connect to the SharePoint site you disabled, and they can no longer link documents from SharePoint to *`Workfront`*.&nbsp;





## Disable custom integrations {#disable-custom-integrations}




1. Log in to *`Workfront`* as the administrator.
1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1.  Click `Documents` > `Custom Integration`.
1. Select the custom&nbsp;integration you want to disable.
1.  Click `Disable`.


   Users are not able to connect to the third-party document provider you disabled, and they can no longer link documents from that cloud provider to *`Workfront`*.



