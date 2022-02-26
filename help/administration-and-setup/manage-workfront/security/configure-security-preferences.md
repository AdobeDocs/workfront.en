---
filename: configure-security-preferences
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Configure system security preferences
description: The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Admin Console.
---

# Configure system security preferences

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Admin Console.
>
>If your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

As an *Adobe Workfront administrator*, you can configure security preferences for your *Workfront* system:

* Access to *Workfront* from mobile apps and other integrated applications
* Rules for embedding *Workfront* in an iframe

Changes that you make in the system preferences impact all users in your system, and their experience in *Workfront*.

We recommend that you configure your system security preferences during the *Workfront* implementation and only occasionally revisit them after that.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <em>Workfront administrator</em>. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configure your system security preferences

<ol> <draft-comment>
  <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li>
 </draft-comment>
 <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">In the left panel, click <span class="bold">System</span> > <span class="bold">Preferences</span>.<br></li> 
 <li value="3"> <p>In the <span class="bold">Security</span> section, select any of the following fields to establish the security settings for your organization:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader"> <p>Allow embedding of <span class="bold">Workfront</span> in an iframe</p> </td> 
     <td>Lets you embed <em>Workfront</em> in an iframe.<p>This option is disabled by default.</p><note type="important">
       Displaying a web-based application in an iframe makes the application susceptible to a click-jacking security vulnerability.
      </note></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Allow SAML 2.0 authentication in Office 365 add-ins</td> 
     <td> <p>Lets you embed <em>Workfront</em> in an iframe only for Office 365 add-ins when <em>Workfront</em> is integrated with a SAML 2.0 single sign-on solution. </p> <p>This option is enabled by default.</p> <note type="note">
        If you enable the option above, 
       <span class="bold">Allow embedding of Workfront in an iframe</span>, the option 
       <span class="bold">Allow SAML 2.0 authentication in Office 365 add-ins</span> is enabled and dimmed.
       <br>
      </note> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Enable the use of session information when creating External Page URLs</td> 
     <td> <p>Allows users to use the Session ID information of a site when adding an External Page to a Dashboard.<br></p> <p>For more information about adding External Pages to a Dashboard, see <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">Embed an external web page in a dashboard</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Let people use Workfront's mobile applications and the <span class="bold">Workfront</span> Outlook Add-In</td> 
     <td> <p>Allows users to access the mobile apps (<em>Workfront</em> View for iPad and mobile phone apps) and the <em>Workfront</em> Outlook app.</p> <p>This option is enabled by default. </p> <p>For information about <em>Workfront</em> View, see <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Use Adobe Workfront View</a>. For more information about the mobile apps, see <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Use the Adobe Workfront mobile app</a>.</p> <p>For more information about the Outlook plugin, see <a href="../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md" class="MCXref xref">Set up Adobe Workfront for Outlook</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"> <p>Collaborate with people without Workfront accounts by using email addresses</p> </td> 
     <td>Allows <em>Workfront</em> users to share certain items with people without a <em>Workfront</em> account by including their email address instead of their name. Users can share the following items with external users by using their email address:
      <ul>
       <li>Document<br></li>
       <li>Document request<br></li>
       <li>Document approval</li>
       <li>Calendar</li>
      </ul><p>This option is enabled by default.</p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Require external users to register with a password</td> 
     <td> <p>Requires external users to register before they are able to view items in <em>Workfront</em>. By default, this option is disabled. When you enable this option, people without a <em>Workfront</em> account who are included in certain updates by their email address, will be prompted to create an account before they can view the item they are included on. This creates an External User account for them.</p> <p>This option is disabled by default.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Automatically log users out after</td> 
     <td> <note type="note">
       This is not currently available. We are working on authentication enhancements that will allow you to log out inactive users automatically after a period of time that you choose.
      </note> <p>Lets you specify when a user is logged out of <em>Workfront</em>, after a period of inactivity. By default, users are logged out after 8 hours of inactivity. </p> <p>This option also affects <em>Workfront</em> customers who are using a single sign-on solution.</p> <note type="note">
       This is not available if your organization’s 
       <em>Workfront</em> instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.
      </note> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Automatically log mobile users out after </td> 
     <td>Lets you specify when a user is logged out of the <em>Workfront</em> application, after a period of inactivity. By default, users are logged out after 7 days of inactivity. <p>This option also affects <em>Workfront</em> customers who are using a single sign-on solution.</p></td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Enable Zoom integration in the updates stream</span> </td> 
     <td> <p>Lets you enable or disable the Zoom integration in the Updates area for all users in the organization.<br>The Zoom integration allows users to add a Zoom meeting URL to a comment or reply in the Updates area. For more information, see <a href="https://one.workfront.com/s/article/Using-the-Zoom-integration?language=en_US">Using the Zoom integration</a>. Also see the section <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add" class="MCXref xref">Add an update to a work item</a> in the article<a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Update work</a>.</p> <p>Users can uninstall the Zoom integration in their personal instance of <em>Workfront</em>. For more information, see <a href="https://one.workfront.com/s/article/Uninstalling-the-Zoom-integration?language=en_US">Uninstalling the Zoom integration</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="4"> <p>Click <span class="bold">Save</span>.</p> <p>The changes that you saved here affect the experience of all the users in <em>Workfront</em> and anyone who interacts with them as an external user.</p> </li> 
</ol>

