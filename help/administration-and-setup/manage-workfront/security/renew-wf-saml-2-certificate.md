---
filename: renew-wf-saml-2-certificate
user-type: administrator
product-area: system-administration
keywords: SAML 2.0,security,certificate,Admin,Exemption,configure,metadata
navigation-topic: security
title: Renew the Adobe Workfront SAML 2.0 metadata certificate
description: The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
---

# Renew the *Adobe Workfront* SAML 2.0 metadata certificate

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on performing this action in the Adobe Admin Console, see "The digital signature in the SAML response did not validate with the identity provider's certificate" in [Troubleshooting errors](https://helpx.adobe.com/enterprise/kb/tshoot-fed-id.html), or reach out to your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

The *Adobe Workfront* servers utilize the SAML 2.0 protocol for authentication and authorization. Once updated, the new certiﬁcate remains valid for one year. When it is time for you to renew the certiﬁcate on your identity provider, you receive a warning in Workfront alerting you that this change must occur. As a *Workfront administrator*, you can manage this change at the system level.

In 2021, our SAML 2.0 metadata certiﬁcate expired on October 27. The next date when we plan to update the certiﬁcate is November 22, 2022.

>[!IMPORTANT]
>
>You must take action to update the metadata in your identity provider with the information from the renewed certiﬁcate before the speciﬁed date. Mismatched certiﬁcates can keep your users from logging in to *Workfront* after November 22, 20221.>
><!-->
><span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Use this message in the last few weeks before the update.</span>>
>-->
>`Use this message in the last few weeks before the update.`

>[!NOTE]
>
>This is not available if your organization’s *Workfront* instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

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

## Configure SAML 2.0 within *Workfront*

To review the warning message and acknowledge the update of the SAML 2.0 metadata in your identity provider:

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">Click <span class="bold">System</span> > <span class="bold">Single Sign-On</span>.</li> 
 <li value="3">In the <span class="bold">Type</span> drop-down menu, select <span class="bold">SAML 2.0</span>.</li> 
 <li value="4"> <p>Click <span class="bold">Download SAML 2.0 Metadata</span>.</p> <p>This downloads the renewed <em>Workfront</em> certiﬁcate for SAML 2.0, which contains the correct metadata for your server.</p> 
  <div class="warning" data-mc-autonum="<b>Warning: </b>">
   <span class="autonumber"><span><b>Warning: </b></span></span> 
   <p>Before you upload the <em>Workfront</em> metadata to your Single Sign-On (SSO) provider in Step 5, copy your current Assertion Consumer Service (ACS) URL to a safe place. This URL, also known as the Reply URL, is found on your SSO provider's <em>Workfront</em> configuration page. </p> 
   <p>If the ACS URL changes after you upload the <em>Workfront</em> metadata, this means that the metadata might contain an incorrect ACS URL. You must change it back to the one you copied in order to avoid breaking your Single Sign-On connection. Your updated certificate will still be correct after you do this.</p> 
  </div> </li> 
 <li value="5">Go to your identity provider server and update the new certiﬁcate you downloaded from <em>Workfront</em> on that server, as explained in <a href="../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md" class="MCXref xref">Update SAML 2.0 metadata in your identity provider</a>.</li> 
 <li value="6"> <p>In <em>Workfront</em>, on the <b>Single Sign-on (SSO) page</b>, make sure that <span class="bold">Admin Exemption</span> is selected.</p> <p>When this ﬁeld is selected, <em>Workfront administrators</em> can log in to <em>Workfront</em> with their SSO credentials or their <em>Workfront</em> credentials.</p> </li> 
 <li value="7"> <p>Click <span class="bold">Save</span>.</p> <p>The warning message no longer displays because you acknowledged the renewal of the SAML 2.0 certiﬁcate on the server of your identity provider.</p> </li> 
 <li value="8"> <p>Click <span class="bold">Test Connection</span> to test your conﬁguration.</p> <p>You should see a message confirming that the connection was successful.</p> </li> 
</ol>

For more information, or for assistance with the manual conﬁguration of metadata, please contact our Support Team, as explained in [Contact Customer Support](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
