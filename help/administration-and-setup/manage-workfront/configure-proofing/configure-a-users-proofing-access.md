---
filename: configure-a-users-proofing-access
user-type: administrator
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: Configure a user's proofing access
description: The sections in this article shouldn't be lumped together.
---

# Configure a user's *proofing* access

<!--
<p style="color: #000000;" data-mc-conditions="QuicksilverOrClassic.Draft mode">The sections in this article shouldn't be lumped together. </p>
-->

The sections in this article shouldn't be lumped together.

<!--
<p style="color: #000000;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> -------------Also, need to add a bit of info to the bottom section about how you can view interactive content in screen sizes but not emulated.</p>
-->

-------------Also, need to add a bit of info to the bottom section about how you can view interactive content in screen sizes but not emulated.

As a *Adobe Workfront administrator* or *Workfront Proof administrator*, you can configure a user's access to create and view *proofs* in *Workfront* and *Workfront Proof*.

For information about *proofing* functionality available for basic and integrated *proofing*, see [Access to proofing functionality in Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>You must be a <em>Workfront administrator</em> or <em>Workfront Proof administrator</em>. For information on <em>Workfront administrators</em>, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Enable and disable *proofing* for&nbsp;a user (legacy plans only)

If your organization is using a legacy Select or Premium Workfront Plan, as a *Workfront administrator*, you can enable and disable *proofing* functionality for the user.

When you enable *proofing* for a user, *Workfront* enables the option for the user's *proofs* to generate automatically. For more information about this option and how to disable it, see [Configure a user's proofing access](#).&nbsp;

Though you can enable a user as a *proofing* user, he or she must have Administrator permissions in order to navigate directly to the *Workfront Proof* interface from the *Workfront* 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Main Menu
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Main Menu</MadCap:conditionalText>`. For information about how you can enable this option for all *proofing* users in your *Workfront* system, see [Configure Workfront Proof access via Workfront Main Menu for all users](#configuring-whether-all-users-can-access-proofhq-directly-from-the-workfront-global-nav).

   <!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver">In the <span class="bold">Main Menu</span>, select <span class="bold">Users</span>.</li>
   -->

1. In the `Main Menu`, select `Users`.

   <!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Select a user, then click the <span class="bold">Edit</span> icon.</li>
   -->

1. Select a user, then click the `Edit` icon.
1. In the `Access` section, select or deselect `User can generate proofs`.

## Configure a user's *proof* permission profile

The permission profile you select is granted to the users for each *proof* that exists within your organization.

<ol> 
 <li value="1"> <p>Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Users</span> <img src="assets/users-icon-in-main-menu.png">. </p> </li> 
 <li value="2"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Select one or more users, then click <span class="bold">Edit</span>.<br></p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Select one or more users, then click <span class="bold">Edit</span>.<br></p> </li> 
 <li value="3"> <p>In the <span class="bold">Access</span> section, click one of the following <em>Workfront Proof</em> permission options in the <span class="bold">Proof Permission Profile</span>&nbsp;drop-down menu:</p> <note type="note">
   If you are on a legacy Workfront plan, make sure the 
   <span class="bold">User can generate proofs</span> option is enabled, as explained above in the section 
   <a href="#enabling-and-disabling-proofing-for-a-user" class="MCXref xref">Enable and disable proofing for&nbsp;a user (legacy plans only)</a>.&nbsp;
  </note> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader"><span class="bold">Supervisor</span> </td> 
     <td>Users can manage and view all <em>proofs</em> created on your organization's account. They can also edit reviewers added to these <em>proofs</em>. Users with this permission profile can't manage users or edit <em>Workfront Proof</em> settings.</td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Manager</span> </td> 
     <td> <p> Users can manage and view <em>proofs</em> created or owned on your organization's account. They can view other users' <em>proofs</em> only when added as a reviewer. This is a default setting. </p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Administrator</span> </td> 
     <td> Users are given Administrator permissions in <em>Workfront Proof</em> and can edit account settings. Users can manage and view all <em>proofs</em> created on your organization's account. This includes adding and removing reviewers, <em>proofs</em>, and comments.</td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Custom</span> </td> 
     <td> <p>Available only if you have configured a custom permission profile within <em>Workfront Proof</em>.</p> <note type="note"> 
       <p>Ensure that the permission profile you grant here does not provide higher access than the user's&nbsp;Access Level&nbsp;setting in <em>Workfront</em> (see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>). If it does provide higher&nbsp;access, the user can access <em>proofs</em> within <em>Workfront Proof</em> that he or she cannot access within <em>Workfront</em>.</p> 
       <p>This is especially important if you plan to allow all <em>Workfront</em> users to access <em>Workfront Proof</em> directly from the <em>Workfront</em> as described in&nbsp;<a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">Access Workfront Proof from Adobe Workfront</a>.</p> 
       <p>By default, only <em>Workfront</em> administrators have access to a direct link to the <em>Workfront Proof</em> site from the <em>Workfront</em> Global Navigation Bar.</p> 
      </note> </td> 
    </tr> 
   </tbody> 
  </table> <p>The permission profile you select is granted to the users for each <em>proof</em> that exists within your organization.</p> </li> 
 <li value="4"> <p>Click <span class="bold">Save Changes</span>&nbsp;to complete the update to the user settings.</p> <note type="note">
   When you create or update a user in 
   <em>Workfront</em> and the user's 
   <em>Workfront</em> email address matches that of a licensed 
   <em>Workfront Proof</em> user, the system enables 
   <em>proofing</em> for the user within 
   <em>Workfront</em>.&nbsp;For more information, see 
   <a href="../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md" class="MCXref xref">User synchronization between Adobe Workfront and Workfront Proof</a>.
  </note> </li> 
</ol>

### Considerations

Consider the following information when setting permissions:

* If you change a user's&nbsp;permission profile to a profile with fewer permissions, the user might lose visibility to existing *proofs* within *Workfront*.&nbsp;This can occur when someone shares a task with a user within *Workfront*, but doesn't share the *proof* attached to the task (see&nbsp; [Share a proof within Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)&nbsp;in [Share a proof within Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)).
* You can set *Workfront Proof* permissions from *Workfront*&nbsp;only if your *Workfront* environment is integrated with a *Workfront Proof* Premium account. If you cannot use *proofing* as discussed in this section, contact your *Workfront administrator*.
* At least one user in your *Workfront* environment must have Administrator permissions for&nbsp;*proofing*. An error message appears if you try to attempt to remove Administrator permissions for *proofing* from all users.
* When you change a user's *Workfront* Access level to any level other than System Administrator, the user's *Workfront Proof* permission profile defaults to Manager.   

* When you change the *Workfront* Access level to System Administrator, the Proof Permission profile changes to Administrator.

## Configure *Workfront Proof* access via *Workfront* 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Main Menu
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Main Menu</MadCap:conditionalText>` for all users

By default, only users with administrative rights within *Workfront* can access *Workfront Proof* as described&nbsp; [Access Workfront Proof from Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

You can grant all users access to the *Workfront Proof* button within the *Workfront* 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Main Menu
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Main Menu</MadCap:conditionalText>` by contacting *Workfront* Support and submitting a request.

>[!IMPORTANT]
>
>&nbsp;If you plan to allow all *Workfront* users to access *Workfront Proof* directly from the *Workfront* Global Navigation Bar,&nbsp;ensure that the permission profile for each user does not provide more access than the user's access level within *Workfront*. This prevents users from accessing *proofs* within *Workfront Proof* that they cannot access within *Workfront*. For more information, see [Enable and disable proofing for a user (legacy plans only)](#enabling-and-disabling-proofing-for-a-user).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode"><a name="configuring-whether-users-can-access-the-html5-proofing-viewer"></a>Configure user access to <em>Web Proofing Viewer</em></h2>
-->

## Configure user access to *Web Proofing Viewer*

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The <em>Web Proofing Viewer</em> launches by default when users in your organization <em>proof</em> video and static content.</p>
-->

The *Web Proofing Viewer* launches by default when users in your organization *proof* video and static content.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">As the <em>Workfront administrator</em>, if your organization opted to use the Legacy <em>proofing viewer</em> as the default until it is removed, you can switch the default for your users to the <em>Web Proofing Viewer</em>.&nbsp;</p>
-->

As the *Workfront administrator*, if your organization opted to use the Legacy *proofing viewer* as the default until it is removed, you can switch the default for your users to the *Web Proofing Viewer*.&nbsp;

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You might not have access to the Legacy <em>proofing viewer</em> because it is supported by Flash, which has been deprecated in most environments.</p>
-->

You might not have access to the Legacy *proofing viewer* because it is supported by Flash, which has been deprecated in most environments.

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1"> <p>From <em>Workfront</em>, click the <em>Workfront Proof</em> icon in the Global Navigation Bar to access <em>Workfront</em> Proof.</p> <p> <img src="assets/proof-access-proofhq-350x39.png" alt="" style="width: 350;height: 39;"> </p> </li>
<li value="2">Click <span class="bold">Account settings</span> near the upper-right corner of <em>Workfront Proof</em>, then click the <span class="bold">Settings</span> tab.</li>
<li value="3">Under <span class="bold">Proof Defaults</span>, at the end of the <span class="bold">New Proofing Viewer for video and static proofs</span> row, click <span class="bold">Setup</span>.</li>
<li value="4">Modify the <em>Web Proofing Viewer</em> settings, as explained under <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#web-proofing-viewer" class="MCXref xref">Web Proofing Viewer</a> in the article <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md" class="MCXref xref">Configure proof settings for your organization</a>.</li>
<li value="5">Click <span class="bold">Save</span>.&nbsp;</li>
</ol>
-->

<ol data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
 <li value="1"> <p>From <em>Workfront</em>, click the <em>Workfront Proof</em> icon in the Global Navigation Bar to access <em>Workfront</em> Proof.</p> <p> <img src="assets/proof-access-proofhq-350x39.png" alt="" style="width: 350;height: 39;"> </p> </li> 
 <li value="2">Click <span class="bold">Account settings</span> near the upper-right corner of <em>Workfront Proof</em>, then click the <span class="bold">Settings</span> tab.</li> 
 <li value="3">Under <span class="bold">Proof Defaults</span>, at the end of the <span class="bold">New Proofing Viewer for video and static proofs</span> row, click <span class="bold">Setup</span>.</li> 
 <li value="4">Modify the <em>Web Proofing Viewer</em> settings, as explained under <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#web-proofing-viewer" class="MCXref xref">Web Proofing Viewer</a> in the article <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md" class="MCXref xref">Configure proof settings for your organization</a>.</li> 
 <li value="5">Click <span class="bold">Save</span>.&nbsp;</li> 
</ol>

## Configure user access to the *Desktop Proofing Viewer*

If the users in your organization would prefer to use the *Desktop Proofing Viewer* instead of the *Web Proofing Viewer* to review interactive content, you can configure the *Desktop Proofing Viewer* to launch automatically when users open interactive content proofs.&nbsp;For information about this the *Desktop Proofing Viewer* and how it differs from the *Web Proofing Viewer*, see [Understand the Desktop Proofing Viewer](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md) and [Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

<ol> 
 <li value="1"> <p>From <em>Workfront</em>, click the <em>Workfront Proof</em> icon in the Global Navigation Bar to access <em>Workfront</em> Proof.</p> <p> <img src="assets/proof-access-proofhq-350x39.png" alt="" style="width: 350;height: 39;"> </p> </li> 
</ol>

1. Click `Account settings` near the upper-right corner of *Workfront Proof*, then click the `Settings` tab.

1. Under `Proof Defaults`, at the end of the `*Desktop Proofing Viewer* for Interactive *proofing*` row, click `Setup`.

1. Modify the *Desktop Proofing Viewer* settings, as described in [Desktop Proofing Viewer](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#desktop-proofing-viewer) in the article [Configure proof settings for your organization](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).

1. Click `Save`.

## Configure custom devices for interactive proofs

You can&nbsp;add any custom devices to your system, allowing users to review interactive content and simulate how the content appears on a specific device when they are using the *Desktop Proofing Viewer*. (This functionality is not available in the *Web Proofing Viewer*, where users can review&nbsp;interactive content, but only as it appears in various resolutions, not on various devices.)

For more information, see [Change interactive proof resolution in the proofing viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

1. From *Workfront*, access the *Workfront Proof* interface, as described in [Access Workfront Proof from Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

1. Modify the *Desktop Proofing Viewer* settings, as described in [Configure custom devices for proofs](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#custom-devices-for-proofs) in the article [Configure proof settings for your organization](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md). `  
   `

