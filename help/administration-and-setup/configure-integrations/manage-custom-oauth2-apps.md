

# View and manage custom OAuth2 applications

As an Adobe Workfront administrator, you can view and manage the OAuth2 applications for your instance of Workfront, which allow other applications to access Workfront.

>[!NOTE]
>
>In the context of OAuth2, "Oauth2 application: refers to the this sort of access link between an app and a server such as Workfront. 
>
>For more information, see [Create OAuth2 applications for Workfront integrations](../../administration-and-setup/configure-integrations/create-oauth-application.md)

* For information on creating custom OAuth2 applications, see [Create OAuth2 applications for Workfront integrations](../../administration-and-setup/configure-integrations/create-oauth-application.md)
* For instructions on configuring and using the OAuth2 application with user credentials (authorization code flow), see [Configure and use your organization's custom OAuth 2 applications using authorization code flow](../../wf-api/api/oauth-app-code-token-flow.md).
* For instructions on configuring and using the OAuth2 application using server authentication (JWT flow), see [Configure and use your organization's custom OAuth 2 applications using JWT flow](../../wf-api/api/oauth-app-jwt-flow.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Planor higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <!--
     You must be a Workfront administrator.
    --> <!--
     For information on Workfront administrators, see Grant a user full administrative access.
    --> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

You must create OAuth2 applications for your organization before you can view or manage them.

For more information, see [Create OAuth2 applications for Workfront integrations](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## Manage custom OAuth2 applications

* [View and edit custom OAuth2 applications](#view) 
* [Delete custom OAuth2 Applications](#delete)

### View and edit custom OAuth2 applications

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2"> <p>In the left navigation panel, click <b>System</b>, then select <b>OAuth Applications</b>.</p> </li> 
 <li value="3"> <p>Click <b>Create app integration</b>.</p> </li> 
 <li value="4"> <p>Hover over the application and click the <b>Edit</b> icon when it appears on the far right.</p> </li> 
 <li value="5"> <p>(Optional) Edit any details of the application. </p> <p>For fields related to OAuth2 and JWT apps, see <a href="../../administration-and-setup/configure-integrations/create-oauth-application.md" class="MCXref xref">Create OAuth2 applications for Workfront integrations</a></p> </li> 
</ol>

### Delete custom OAuth2 Applications

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2"> <p>In the left navigation panel, click <b>System</b>, then select <b>OAuth Applications</b>.</p> </li> 
 <li value="3"> <p>Click <b>Create app integration</b>.</p> </li> 
 <li value="4"> <p>Hover over the application and click the <b>Delete</b> icon when it appears on the far right.</p> </li> 
</ol>

## Manage Client Secrets in OAuth2 applications

* [View Client Secret details](#view2) 
* [Add or edit notes for Client Secret](#add) 
* [Delete Client Secret](#delete2)

### View Client Secret details

>[!IMPORTANT]
>
>You cannot view the Client Secret itself. If you have lost your client secret, you must delete it and create a new one.
>
>* To delete a Client Secret, see [Delete Client Secret](#delete2) in this article.
>* To create a new Client Secret, see [Create an OAuth2 application](../../administration-and-setup/configure-integrations/create-oauth-application.md#create) in [Create OAuth2 applications for Workfront integrations](../../administration-and-setup/configure-integrations/create-oauth-application.md).
>

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2"> <p>In the left navigation panel, click <b>System</b>, then select <b>OAuth Applications</b>.</p> </li> 
 <li value="3"> <p>Click <b>Create app integration</b>.</p> </li> 
 <li value="4"> <p>Hover over the application and click the <b>Edit</b> icon when it appears on the far right.</p> </li> 
 <li value="5"> <p>View details in the Client Secret area:</p> 
  <ul> 
   <li> <p>Created date</p> </li> 
   <li> <p>Last used date</p> </li> 
   <li> <p>Notes </p> <p>To add notes to a Client Secret, see <a href="#add" class="MCXref xref">Add or edit notes for Client Secret</a>.</p> </li> 
  </ul> </li> 
</ol>

### Add or edit notes for Client Secret

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2"> <p>In the left navigation panel, click <b>System</b>, then select <b>OAuth Applications</b>.</p> </li> 
 <li value="3"> <p>Click <b>Create app integration</b>.</p> </li> 
 <li value="4"> <p>Hover over the application and click the <b>Edit</b> icon when it appears on the far right.</p> </li> 
 <li value="5"> <p>Locate the Client Secret that you want to add or edit a note for.</p> </li> 
 <li value="6"> <p>Click the box that contains details for the Client Secret.</p> <p>You can now add note text, or edit existing note text.</p> <note type="note">
   Note text has a maximum of 64 characters.
  </note> </li> 
 <li value="7"> <p>Click out of the box or press <b>Enter</b> to save the note text.</p> </li> 
</ol>

### Delete Client Secret

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2"> <p>In the left navigation panel, click <b>System</b>, then select <b>OAuth Applications</b>.</p> </li> 
 <li value="3"> <p>Click <b>Create app integration</b>.</p> </li> 
 <li value="4"> <p>Hover over the application and click the <b>Edit</b> icon when it appears on the far right.</p> </li> 
 <li value="5"> <p>Locate the Client Secret that you want to delete.</p> </li> 
 <li value="6"> <p>Click the <b>Delete</b> icon <img src="assets/delete.png"> next to the Client Secret.</p> </li> 
</ol>

