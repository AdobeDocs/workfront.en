---
filename: change-your-workfront-domain
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Change your Adobe Workfront domain
description: As an Adobe Workfront administrator and an authorized Workfront Support contact, you can request help from the Workfront Support team to change your organization's Workfront domain.
---

# Change your *Adobe Workfront* domain

As an *Adobe Workfront administrator* and an authorized *Workfront* Support contact, you can request help from the *Workfront* Support team to change your organization's *Workfront* domain.

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

## Request a domain change

1. Click the `Support` tab on the Workfront One page, then start creating a support case.
1. In the `Description` box, include the new new domain you want, as well as the timeframe when you want the new domain to go live.
1. Finish filling out the boxes for the support case, then click `Submit`.

You can also call Workfront Support to get help changing your domain.

## Update the new domain if you are an SSO customer

If your company utilizes SSO, the following steps are required after you have your *Workfront* domain changed.

>[!NOTE]
>
>This is not available if your organization’s *Workfront* instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">In the left sidebar, click <span class="bold">System</span> > <span class="bold">Customer Info</span> and make sure that your domain is updated on the Customer Info page.</li> 
 <li value="3">In the left sidebar, click <span class="bold">System</span> > <span class="bold">Single Sign-On (SSO)</span>.</li> 
 <li value="4">Click <span class="bold">Download SAML 2.0 Metadata</span>.</li> 
 <li value="5">After the file is downloaded, open it and make sure of the following:
  <ol>
   <li value="1"><span class="bold">entityID</span> is pointing to the new domain.</li>
   <li value="2">All locations within <span class="bold"><md:AssertionConsumerService></span> point to the new domain.</li>
  </ol></li> 
 <li value="6">Provide the downloaded metadata file to your Identity Provider so that they can update it on their end.</li> 
 <li value="7">Make sure the domain is updated for all <em>Workfront</em> integrations used by your organization.</li> 
</ol>

