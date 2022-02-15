


# Call the MS Graph REST API via the HTTP > Make an OAuth 2.0 request module {#call-the-ms-graph-rest-api-via-the-http-make-an-oauth-request-module}

Many Microsoft web services are accessed through the Microsoft Graph API. This article describes how to create a connection to that API, using the *`Workfront Fusion`* HTTP > Make an OAuth 2.0 request module.


## Access requirements {#access-requirements}

You must have the following access to use the functionality in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p><span class="mc-variable WFVariables.WFPlan-Pro variable varname">Pro</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWFF variable varname">Adobe Workfront Fusion</span> license**</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFFusionIntegration variable varname">Workfront Fusion for Work Automation and Integration</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Product</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Your organization must purchase <span class="mc-variable WFVariables.FullProdNameWFF variable varname">Adobe Workfront Fusion</span> as well as <span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Register *`Workfront Fusion`* in the Microsoft Application Registration Portal {#register-workfront-fusion-in-the-microsoft-application-registration-portal}

To create a connection to the Microsoft Graph REST API, you must first register *`Adobe Workfront Fusion`*.



1.  Begin registering a new application as described in [Register your app](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) in the Microsoft documentation.


   As part of the registration, Microsoft requires the following information:


1.  When you have completed the app registration, make note of the Application ID.


   >[!IMPORTANT] {type="important"}
   >
   >You will need the Application ID to set up your connection in *`Workfront Fusion`*.



1.  Generate an Application Secret. Make note of this secret.


   For instructions, see [Register your app](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) in the Microsoft documentation.


   >[!IMPORTANT] {type="important"}
   >
   >You will need the Application Secret to set up your connection in *`Workfront Fusion`*.



1.  Configure the permissions for your application.


   For specifics on locating and configuring these fields, see the "Configure permissions for Microsoft Graph" section in [Get access without a user](https://docs.microsoft.com/en-us/graph/auth-v2-service) in the Microsoft documentation.

<table style="mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">What type of permissions does your application require?</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Select <code>Delegated permissions</code>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Select permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Select the following permissions:</p> 
    <ul> 
     <li> <p><code>offline_access</code> </p> </li> 
     <li> <p><code>openid</code> </p> </li> 
     <li> <p>Any other permissions required by your integrations (Example: <code>User.Read</code>)</p> </li> 
    </ul> <p>Important: You will need the selected permissions to set up your connection in <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span>.</p> </td> 
  </tr> 
 </tbody> 
</table>


1.  Proceed to [Configure your MS Graph API connection in Workfront Fusion](#configur).




## Configure your MS Graph API connection in *`Workfront Fusion`* {#configure-your-ms-graph-api-connection-in-workfront-fusion}

After you register *`Workfront Fusion`* as discussed in [Register Workfront Fusion in the Microsoft Application Registration Portal](#register), you can configure your connection in the HTTP > Make an Oauth 2.0 request module.



1.  Add an HTTP > Make an OAuth 2.0 call module to your scenario.
1.  Click **Add** next to the connection field.
1.  Configure the connection fields as follows:

<table style="mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Connection name</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Enter a name for the connection.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> <p role="rowheader">Flow type</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><code>Authorization Code</code> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Authorize URI</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><code>https://login.microsoftonline.com/common/oauth2/v2.0/authorize</code> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Token URI</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><code>https://login.microsoftonline.com/common/oauth2/v2.0/token</code> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Scope</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Enter the permissions that you selected in step 4 of <a href="#register" class="MCXref xref">Register Workfront Fusion in the Microsoft Application Registration Portal</a>.</p> <p>For each scope, click <b>Add</b> and type in the permission.</p> <p>Example: <code>offline_access</code>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Scope separator</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><code>SPACE</code> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Client ID</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Enter the Application ID from step 2 in <a href="#register" class="MCXref xref">Register Workfront Fusion in the Microsoft Application Registration Portal</a>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Client Secret</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Enter the Application Secret that you generated in step 2 in <a href="#register" class="MCXref xref">Register Workfront Fusion in the Microsoft Application Registration Portal</a>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Authorize parameters</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Add the following Authorize parameters:</p> 
    <ul> 
     <li> <p>Key:<code> response_mode</code> Value: <code>query</code></p> </li> 
     <li> <p>Key: <code>prompt </code>Value: <code>consent</code></p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Access token parameters</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">You do not need to enter anything into this field.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Refresh token parameters</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> 
    <ol> 
     <li value="1"> <p>Click <b>Add</b>.</p> </li> 
     <li value="2"> <p>In the <b>Key</b> field, enter <code>scope</code>.</p> </li> 
     <li value="3"> <p>In the <b>Value</b> field, enter all of the scopes that you entered into the scope field, separated by spaces.</p> <p>Example: <code>offline_access openid User.Read</code></p> </li> 
    </ol> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Custom Headers</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">You do not need to enter anything into this field.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Token Placement</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"><code>In the header</code> </td> 
  </tr> 
 </tbody> 
</table>


1.  Click **Continue**.
1.  In the window that appears, click **Accept** to complete the connection and return to the module.


