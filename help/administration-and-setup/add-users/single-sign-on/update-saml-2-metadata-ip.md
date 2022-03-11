---
filename: update-saml-2-metadata-ip
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Update SAML 2.0 metadata in your identity provider
description: The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Admin Console.
---

# Update SAML 2.0 metadata in your identity provider

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Admin Console.
>
>If your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

The following sections describe how to update your Security Assertion Markup Language (SAML) 2.0 metadata when using Active Directory Federation Services (ADFS) as your identity provider.

If your organization has been upgraded to the enhanced authentication experience (not yet available for all organizations), see the information in [Update SAML 2.0 metadata in your IDP when using enhanced authentication](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip-eauth-.md).

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <span>Workfront administrator</span>. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Use ADFS as your identity provider

You can update your ADFS metadata prior to `Adobe Workfront` updating the SAML 2.0 certificate or after. If you choose to update the ADFS metadata prior to `Workfront` updating the SAML 2.0 certificate, additional steps are required.

* [Update your ADFS metadata](#updating-your-adfs-metadata) 
* [Force your ADFS metadata to update](#forcing-your-adfst-metadata-to-update)

### Update your ADFS metadata

To set your ADFS metadata to update automatically, complete the steps in this section.

By default, ADFS is configured to automatically check for updates to all of its relying party trust metadata; however, the default is set to poll only every 24 hours. You can change this value with powershell commands.

<ol> 
 <li value="1">Log in to the ADFS server and open the ADFS Management Console. </li> 
 <li value="2">In the left-hand panel, expand <span class="bold">ADFS 2.0,</span> then expand <span class="bold">Trust Relationships.</span></li> 
 <li value="3">Click the <span class="bold">Relying Party Trusts</span> folder.</li> 
 <li value="4"> <p>Select the relying party trust that you previously configured to be used with <span>Workfront</span>, then in the right-hand panel, click<span class="bold"> Update from Federation Metadata</span>.</p> </li> 
 <li value="5"> <p>(Conditional) If this option is dimmed (which means that the relying party trust was previously configured using a metadata file), complete the following. </p> 
  <ol style="list-style-type: lower-alpha;"> 
   <li value="1"> Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
   <li value="2">Click <span class="bold">System</span> > <span class="bold">Single Sign On (SSO)</span>.</li> 
   <li value="3">Click <span class="bold">Edit Settings.</span> </li> 
   <li value="4">Click <span class="bold">Edit Configuration</span>, then select <span class="bold">SAML 2.0</span> in the <span class="bold">Type</span> drop-down list. </li> 
   <li value="5"> <p>Copy the <span class="bold">Metadata URL</span>, which should be similar to the following: </p> <p>https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData</p> </li> 
   <li value="6">On the ADFS server, right-click on the relying party trust that you previously configured, then click <span class="bold">Properties.</span></li> 
   <li value="7">Click the <span class="bold">Monitoring</span> tab, then paste the URL that you copied from <span>Workfront</span> into the <span class="bold">Relying party's federation metadata URL</span> field.</li> 
   <li value="8">Check the options to <span class="bold">Monitor relying party</span> and <span class="bold">Automatically update relying party</span>.</li> 
   <li value="9">Click <span class="bold">OK.</span></li> 
   <li value="10">Select the relying party trust that you previously configured to be used with <span>Workfront</span>; then, in the right-hand panel, click <span class="bold">Update from Federation Metadata.</span></li> 
  </ol> </li> 
 <li class="p1" value="6">Click <span class="bold">OK</span> to ignore the message about some of the content in the federation metadata not being supported by ADFS 2.0.</li> 
 <li class="p1" value="7">Open <span class="bold">Windows Powershell Modules.</span></li> 
 <li class="p1" value="8"> <p>After all the modules load, run the following command in powershell:<br></p> <p><span class="bold">Get-ADFSProperties</span> </p> </li> 
 <li class="p1" value="9"> <p>Look for the value next to <span class="bold">Monitoring Interval.</span></p> <p>It will be a number that represents the number of minutes between polls. The default should be 1440 (1440 minutes = 24 hours).</p> </li> 
 <li class="p1" value="10"> <p>Set a new value by running the following command in powershell:<br></p> <p><span class="bold">Set-ADFSProperties -MonitoringInterval 1</span> <br>This changes the monitoring interval from every 24 hours to every minute. You can change the 1 to another larger value if you want it to poll less frequently.</p> </li> 
 <li class="p1" value="11"> <p>To verify that this is working correctly, use the <span class="bold">Event Viewer</span> to look for the following information in the ADFS2.0 logs: <br></p> <p><span class="bold">Event ID 156 and 157</span> </p> </li> 
</ol>

### Force your ADFS metadata to update

To update your ADFS metadata complete the steps in the following section.

To force metadata to be exchanged between `Workfront` and your SAML 2.0 provider when using Active Directory Federation Services (ADFS):

>[!NOTE]
>
>Some of these changes might need to be done by your IT department.

1. Log in to the ADFS server and open the `ADFS Management Console`.
1. In the left-hand panel, expand `ADFS 2.0`, then expand `Trust Relationships`.

1. Click the `Relying Party Trusts` folder.
1. Select the relying party trust that you previously configured to be used with `Workfront`, then in the right-hand panel, click `Update from Federation Metadata`.

   If this option is dimmed and cannot be selected, complete the following:

   (The option is dimmed only when the relying party trust was previously configured using a metadata file.)

  1. In `Workfront`, in the Setup area, copy the `Metadata URL` from your `Workfront` Single Sign-On setup screen.

     To access the information for the `Metadata URL`:

    1. Click `Setup` near the upper-right corner of `Adobe Workfront` on the Global Navigation Bar.
    1. Click > `System` > `Single Sign On (SSO)`.
    1. Click `Edit Settings.`
    1. Click `Edit Configuration`, then select `SAML 2.0` in the `Type` drop-down list.
    1. Copy the `Metadata URL`, which should be similar to the following:

       *https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData*

  1. On the ADFS server, right-click on the relying party trust that you previously configured, then click `Properties.`
  1. Click the `Monitoring` tab, then paste the URL that you copied from `Workfront` into the `Relying party's federation metadata URL` field.
  1. Check the options to `Monitor relying party` and `Automatically update relying party`.
  1. Click `OK`.
  1. Select the relying party trust that you previously configured to be used with `Workfront`, then in the right-hand panel, click `Update from Federation Metadata.`

1. Click `OK` to ignore the message about some of the content in the federation metadata not being supported by ADFS 2.0.
1. Click `Update` to complete updating your federation metadata.

Users who are allowed to access `Workfront` via the native login screen using `Workfront` login credentials (this can be configured from each user's profile page in the `Access` section) can log in using their `Workfront` user name and password by navigating to the following URL: *https://<yourdomain>.my.workfront.com/ `Workfront`/login.cmd*.

## Using other identity providers

When using identity providers other than ADFS (such as Ping, Okta, or Centrify), you must re-upload the `Workfront` metadata to your identity provider.

For more information about how to obtain a new `Workfront` Metadata URL, see [Update your ADFS metadata](#updating-your-adfs-metadata).

For additional information about using Active Directory Federation Services (ADFS) with SAML 2.0 in `Workfront`, see [Configure Adobe Workfront with SAML 2.0 using ADFS](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
