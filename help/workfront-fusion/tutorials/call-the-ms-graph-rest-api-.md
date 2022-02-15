



# Call the MS Graph REST API  {#call-the-ms-graph-rest-api}

You can call the [Microsoft Graph REST API](https://docs.microsoft.com/en-us/graph/api/overview?view=graph-rest-1.0) from `Workfront Fusion 2.0`:



1. In `Workfront Fusion 2.0`, create a new scenario
1. Insert the HTTP > Make a OAuth 2.0 request module.
1. Open the module's configuration and click **Add** next to the Connection field to create a new connection.
1.  Fill the connection setup as follows:


1. Open the [Microsoft Application Registration Portal](https://login.live.com/login.srf?wa=wsignin1.0&rpsnv=13&ct=1578519809&rver=7.1.6819.0&wp=SAPI_LONG&wreply=https%3a%2f%2fapps.dev.microsoft.com%2fLoginPostBack%3fru%3dhttps%253a%252f%252fapps.dev.microsoft.com%253a443%252f%253freferrer%253dhttps%25253a%25252f%25252fsupport.integromat.com%25252fhc%25252fen-us%25252farticles%25252f360024350193-Calling-Microsoft-Graph-REST-API-via-the-HTTP-Make-a-OAuth-2-0-req&lc=1033&id=293053&aadredir=1) in a new tab/window and log in with your Microsoft account.
1. Under the My applications heading, click on the **Add an app** button.
1. Enter a name (such as 

   ```
   My <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span> App
   ```

   ) and click **Create application**.

1. If you are prompted to view this app in the Azure portal, click **Not now**.
1. Copy the Application Id under the Properties heading, switch to `Workfront Fusion 2.0` and paste it into the Client ID field.
1. Switch back to the Application Registration Portal.
1. Under the Application Secrets heading, click **Generate New Password**.
1. Copy the password, switch to `Workfront Fusion 2.0` and paste it into the Client Secret field.
1. Switch back to the Application Registration Portal.
1. Under the Platforms heading, click **Add Platform**.
1. Choose the Web option.
1. Disable the **Allow Implicit Flow** option.
1. Enter 

   ```
   https://www.workfront.com/oauth/cb/oauth2
   ```

   in the Redirect URLs field.
1.  Under the Microsoft Graph Permissions heading, click **Add** next to the Delegated Permissions and enable the required permissions (refer to the [Microsoft Graph permissions reference](https://docs.microsoft.com/en-us/graph/permissions-reference) for further details).


   For example: 

   ```
   User.Read
   ```

   , 

   ```
   Files.ReadWrite.All
   ```

   .

1. Click **Save** at the bottom of the page.
1. Switch to `Workfront Fusion 2.0`.
1. Add the scopes you added in the previous step into the Scope field.
1. Select the **Show advanced settings** option.
1.  Set the Scope separator to SPACE.


   The connection setup should look like this:


   ![](assets/create-a-connection.png)



1. Click **Continue**.
1.  In the window that appears, review the permissions and click **Accept.**
1.  With the connection now created, configure the module to make an API call.


   See [Microsoft Graph REST API v1.0 reference](https://docs.microsoft.com/en-us/graph/api/overview?view=graph-rest-1.0) for more information.



