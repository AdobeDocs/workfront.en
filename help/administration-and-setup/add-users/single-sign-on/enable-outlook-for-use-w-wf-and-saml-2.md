---
filename: enable-outlook-for-use-w-wf-and-saml-2
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Enable Outlook for use with Workfront and SAML 2.0
description: If you enable SAML 2.0 authentication and you want your users to be able to log in to Workfront from Microsoft Outlook using their SAML 2.0 credentials, you must enable SAML 2.0 to authenticate in Office add-ins.
---

# Enable Outlook for use with Workfront and SAML 2.0

If you enable SAML 2.0 authentication and you want your users to be able to log in to Workfront from Microsoft Outlook using their SAML 2.0 credentials,&nbsp;you must enable SAML 2.0 to authenticate in Office add-ins.

>[!NOTE]
>
>This is not available if your organization’s Workfront instance uses a custom SSO portal>
><!-->
>or is enabled with Adobe IMS>
>-->
>. See your network or IT administrator if you need more information.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Enable Outlook for use with Workfront and SAML 2.0

<ol> 
 <li value="1">Click <span class="bold">Setup</span> near the upper-right corner of Adobe Workfront on the Global Navigation Bar.</li> 
 <li value="2">Click <span class="bold">System</span> > <span class="bold">Preferences</span>.</li> 
 <li value="3"> <p>In the <span class="bold">Security</span> section, make sure that <span class="bold">Allow SAML 2.0 authentication in Office 365 add-ins&nbsp;</span>is enabled.</p> <p>This option enables embedding of Workfront in an Iframe only for Office 365 add-ins. This does not open a click-jacking breach as there is no clickable content involved.</p> <p>This option is enabled by default.</p> <note type="note"> 
   <p>If you enable <span class="bold">Allow embedding of Workfront in an iframe</span>, the <span class="bold">Allow SAML 2.0 authentication in Office 365 add-ins</span> is dimmed and enabled.</p> 
   <p> <img src="assets/o365-iframe-grayed-out-and-general-iframe-checked-350x43.png" alt="" style="width: 350;height: 43;"> </img> </p> 
  </note> </li> 
 <li value="4"> <p>Click <span class="bold">Save</span>.<br></p> <p>The changes that you saved here affect the experience of all the users in Workfront.&nbsp;</p> </li> 
</ol>

