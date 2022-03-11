

# Call the MS Graph REST API via the HTTP > Make an OAuth 2.0 request module

Many&nbsp;Microsoft web services are accessed through the Microsoft Graph API. This article describes how to create a connection to that API, using the Workfront Fusion HTTP > Make an OAuth 2.0 request module.

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> Adobe Workfront license* Plan, Work 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion license**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> <!--
   Access level configurations* You must be a Workfront Fusion administrator for your organization. You must be a Workfront Fusion administrator for your team.
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Register Workfront Fusion in the Microsoft Application Registration Portal

To create a connection to the Microsoft Graph REST&nbsp;API, you must first register Adobe Workfront Fusion.

<ol> 
 <li value="1"> <p>Begin registering a new application as described in <a href="https://docs.microsoft.com/en-us/graph/auth-register-app-v2">Register your app</a> in the Microsoft documentation.</p> <p>As part of the registration, Microsoft requires the following information:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Application name</td> 
     <td>Enter a name for the application, such as "My Workfront Fusion application."</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Redirect URL</td> 
     <td><code>https://app.workfrontfusion.com/oauth/cb/oauth2</code> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="2"> <p>When you have completed the app registration, make note of the Application ID.</p> <note type="important">
   You will need the Application ID to set up your connection in Workfront Fusion.
  </note> </li> 
 <li value="3"> <p>Generate an Application Secret. Make note of this secret.</p> <p>For instructions, see <a href="https://docs.microsoft.com/en-us/graph/auth-register-app-v2">Register your app</a> in the Microsoft documentation.</p> <note type="important">
   You will need the Application Secret to set up your connection in Workfront Fusion.
  </note> </li> 
 <li value="4"> <p>Configure the permissions for your application.</p> <p>For specifics on locating and configuring these fields, see the "Configure permissions for Microsoft Graph" section in <a href="https://docs.microsoft.com/en-us/graph/auth-v2-service">Get access without a user</a> in the Microsoft documentation.</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">What type of permissions does your application require?</td> 
     <td>Select <code>Delegated permissions</code>.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Select permissions</td> 
     <td> <p>Select the following permissions:</p> 
      <ul> 
       <li> <p><code>offline_access</code> </p> </li> 
       <li> <p><code>openid</code> </p> </li> 
       <li> <p>Any other permissions required by your integrations (Example: <code>User.Read</code>)</p> </li> 
      </ul> <note type="important">
       You will need the selected permissions to set up your connection in Workfront Fusion.
      </note> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="5"> <p>Proceed to <a href="#configur" class="MCXref xref">Configure your MS Graph API connection in Workfront Fusion</a>.</p> </li> 
</ol>

## Configure your MS Graph API connection in Workfront Fusion

After you register Workfront Fusion as discussed in [Register Workfront Fusion in the Microsoft Application Registration Portal](#register), you can configure your connection in the HTTP > Make an Oauth 2.0 request module.

<ol> 
 <li value="1"> <p>Add an HTTP > Make an OAuth 2.0 call module to your scenario.</p> </li> 
 <li value="2"> <p>Click <b>Add</b> next to the connection field.</p> </li> 
 <li value="3"> <p>Configure the connection fields as follows:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Connection name</td> 
     <td>Enter a name for the connection.</td> 
    </tr> 
    <tr> 
     <td role="rowheader"> <p role="rowheader">Flow type</p> </td> 
     <td><code>Authorization Code</code> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Authorize URI</td> 
     <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/authorize</code> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Token URI</td> 
     <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/token</code> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Scope</td> 
     <td> <p>Enter the permissions that you selected in step 4 of <a href="#register" class="MCXref xref">Register Workfront Fusion in the Microsoft Application Registration Portal</a>.</p> <p>For each scope, click <b>Add</b> and type in the permission.</p> <p>Example: <code>offline_access</code>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Scope separator</td> 
     <td><code>SPACE</code> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Client ID</td> 
     <td>Enter the Application ID from step 2 in <a href="#register" class="MCXref xref">Register Workfront Fusion in the Microsoft Application Registration Portal</a>.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Client Secret</td> 
     <td>Enter the Application Secret that you generated in step 2 in <a href="#register" class="MCXref xref">Register Workfront Fusion in the Microsoft Application Registration Portal</a>.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Authorize parameters</td> 
     <td> <p>Add the following Authorize parameters:</p> 
      <ul> 
       <li> <p>Key:<code> response_mode</code> Value: <code>query</code></p> </li> 
       <li> <p>Key: <code>prompt </code>Value: <code>consent</code></p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Access token parameters</td> 
     <td>You do not need to enter anything into this field.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Refresh token parameters</td> 
     <td> 
      <ol> 
       <li value="1"> <p>Click <b>Add</b>.</p> </li> 
       <li value="2"> <p>In the <b>Key</b> field, enter <code>scope</code>.</p> </li> 
       <li value="3"> <p>In the <b>Value</b> field, enter all of the scopes that you entered into the scope field, separated by spaces.</p> <p>Example: <code>offline_access openid User.Read</code></p> </li> 
      </ol> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Custom Headers</td> 
     <td>You do not need to enter anything into this field.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Token Placement</td> 
     <td><code>In the header</code> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="4"> <p>Click <b>Continue</b>.</p> </li> 
 <li value="5"> <p>In the window that appears, click <b>Accept</b> to complete the connection and return to the module.</p> </li> 
</ol>

