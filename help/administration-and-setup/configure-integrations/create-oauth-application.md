---
filename: create-oauth-application
title: Disable document integrations
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
---



# Create OAuth2 applications for *`Workfront`* integrations {#create-oauth-applications-for-workfront-integrations}

The information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.


As an *`Adobe Workfront administrator`*, you can create OAuth2 applications for your instance of Workfront, which allow other applications to access *`Workfront`*. Your users can then give permission to those other applications to access their *`Workfront`* data. In this way, you can integrate *`Workfront`* with applications of your choice, including your own in-house applications.


>[!NOTE]
>
>In the context of OAuth2, "creating an app" refers to the process of creating this sort of access link between an app and a server such as *`Workfront`*. 




## OAuth2 overview {#oauth-overview}

Imagine that an application needs to pull some specific information from *`Workfront`*. An application that requests information is called a client. For this example, the client name is ClientApp. ClientApp needs access to a particular user's information, and therefore needs to access *`Workfront`* as that user. If your user gives ClientApp their username and password, ClientApp could access all of the data that the user can access. This is a security risk, because ClientApp only needs a small, specific set of information. 


When you create an OAuth2 app for ClientApp, you are essentially telling *`Workfront`* that ClientApp is allowed to access *`Workfront`*, but it can access only a specific set of information you select, and only if the user whose account ClientApp is accessing gives permission for the access. 


## Create an OAuth2 application {#create-an-oauth-application}




1.  Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).
1.  In the left navigation panel, click **System**, then select **OAuth Applications**.
1.  Click **Create new app**.
1.  Enter a name for the new OAuth2 application, such as "Workfront for ClientApp."
1.  Click **Create**.
1.  Fill in the fields for the new app.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Client ID</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>This field is automatically generated.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Client secret</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>This field is automatically generated</p> <p>Important:  <p>Copy the contents of this field to another secure file before you close this page. You will not be able to see this secret key again.</p> <p>If you lose this key, delete it and create a new Client Secret.</p> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Redirect URLs</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Users will be redirected to this path after they have authenticated with <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>. The path will be appended with the authorization code for access, and must have a protocol.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Logo</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">You can add a logo to make this app more identifiable. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Name</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">This is the same name that you gave the app. This field cannot be empty.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Description</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Enter a description for the integration.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">App Description URL</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">This can be a link to an "About us" page or a page with more information about the integration.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Status</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">This is the current status of the integration.</td> 
  </tr> 
 </tbody> 
</table>


1.  Click **Save**.


&nbsp;


&nbsp;
