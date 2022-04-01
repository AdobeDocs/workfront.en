---
filename: renew-wf-saml-2-certificate
user-type: administrator
product-area: system-administration
keywords: SAML 2.0,security,certificate,Admin,Exemption,configure,metadata
navigation-topic: security
title: Renew the Adobe Workfront SAML 2.0 metadata certificate
description: The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
---

# Renew the Adobe Workfront SAML 2.0 metadata certificate

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on performing this action in the Adobe Admin Console, see "The digital signature in the SAML response did not validate with the identity provider's certificate" in [Troubleshooting errors](https://helpx.adobe.com/enterprise/kb/tshoot-fed-id.html), or reach out to your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

The Adobe Workfront servers utilize the SAML 2.0 protocol for authentication and authorization. Once updated, the new certiﬁcate remains valid for one year. When it is time for you to renew the certiﬁcate on your identity provider, you receive a warning in Workfront alerting you that this change must occur. As a Workfront administrator, you can manage this change at the system level.

In 2021, our SAML 2.0 metadata certiﬁcate expired on October 27. The next date when we plan to update the certiﬁcate is November 22, 2022.

<!--
<note type="important">
You must take action to update the metadata in your identity provider with the information from the renewed certiﬁcate before the speciﬁed date. Mismatched certiﬁcates can keep your users from logging in to Workfront after November 22, 20221.
<!--
<span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Use this message in the last few weeks before the update.</span>
-->
</note>
-->

>[!NOTE]
>
>This is not available if your organization’s Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

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

## Configure SAML 2.0 within Workfront

To review the warning message and acknowledge the update of the SAML 2.0 metadata in your identity provider:

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click **System** > **Single Sign-On**.

1. In the **Type** drop-down menu, select **SAML 2.0**.

1. Click **Download SAML 2.0 Metadata**.

   This downloads the renewed Workfront certiﬁcate for SAML 2.0, which contains the correct metadata for your server.

   >[!CAUTION]
   >
   >Before you upload the Workfront metadata to your Single Sign-On (SSO) provider in Step 5, copy your current Assertion Consumer Service (ACS) URL to a safe place. This URL, also known as the Reply URL, is found on your SSO provider's Workfront configuration page. 
   >
   >
   >If the ACS URL changes after you upload the Workfront metadata, this means that the metadata might contain an incorrect ACS URL. You must change it back to the one you copied in order to avoid breaking your Single Sign-On connection. Your updated certificate will still be correct after you do this.

1. Go to your identity provider server and update the new certiﬁcate you downloaded from Workfront on that server, as explained in [Update SAML 2.0 metadata in your identity provider](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).
1. In Workfront, on the **Single Sign-on (SSO) page**, make sure that **Admin Exemption** is selected.

   When this ﬁeld is selected, Workfront administrators can log in to Workfront with their SSO credentials or their Workfront credentials.

1. Click **Save**.

   The warning message no longer displays because you acknowledged the renewal of the SAML 2.0 certiﬁcate on the server of your identity provider.

1. Click **Test Connection** to test your conﬁguration.

   You should see a message confirming that the connection was successful.

For more information, or for assistance with the manual conﬁguration of metadata, please contact our Support Team, as explained in [Contact Customer Support](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
