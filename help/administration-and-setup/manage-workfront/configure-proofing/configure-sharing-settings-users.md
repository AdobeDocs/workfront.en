---
filename: configure-sharing-settings-users
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Configure sharing settings for your users
description: As an Adobe Workfront administrator or Workfront Proof administrator, you can configure the user accounts with which proofs can be shared, whether users can see all versions of a proof, and the timing when users gain access to shared items.
---

# Configure sharing settings for your users

As an *Adobe Workfront administrator* or *Workfront Proof administrator*, you can configure the user accounts with which *proofs* can be shared, whether users can see all versions of a *proof*, and the timing when users gain&nbsp;access to shared items.&nbsp;

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank"><em>Adobe Workfront</em> plan</a> </td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access configurations</td> 
   <td> <p>You must have Administrator selected in your <em>Proof</em> Permission Profile. For more information, see <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Configure a user's proofing access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Configure sharing with other accounts&nbsp;

<ol> 
 <li value="1"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     From 
    <em>Workfront</em>, click the Main Menu 
    <img src="assets/main-menu-icon.png">, then click Proofing 
    <img src="assets/proofing-in-main-menu.png"> to access 
    <em>Workfront Proof</em>. 
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    From 
   <em>Workfront</em>, click the Main Menu 
   <img src="assets/main-menu-icon.png">, then click Proofing 
   <img src="assets/proofing-in-main-menu.png"> to access 
   <em>Workfront Proof</em>. 
  </MadCap:conditionalText> <br> </li> 
 <li value="2">Click <span class="bold">Settings</span> > <span class="bold">Account settings</span>, then click the <span class="bold">Settings</span> tab.</li> 
 <li value="3">In the <span class="bold">Sharing</span> section, to the right of <span class="bold">Allow sharing with</span>, click <span class="bold">Setup</span>.</li> 
 <li value="4">In the drop-down list that appears, select an option to specify whether you want to make <em>proofs</em> available to anyone, restrict the sharing of your <em>proofs</em> to your own account only, or restrict it to your own account and any partner accounts you're collaborating with.</li> 
 <li value="5">Click <span class="bold">Save.</span></li> 
</ol>

## Configure visibility to all versions of a shared *proof*

<ol> 
 <li value="1"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     From 
    <em>Workfront</em>, click the Main Menu 
    <img src="assets/main-menu-icon.png">, then click Proofing 
    <img src="assets/proofing-in-main-menu.png"> to access 
    <em>Workfront Proof</em>. 
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    From 
   <em>Workfront</em>, click the Main Menu 
   <img src="assets/main-menu-icon.png">, then click Proofing 
   <img src="assets/proofing-in-main-menu.png"> to access 
   <em>Workfront Proof</em>. 
  </MadCap:conditionalText> <br> </li> 
 <li value="2">Click <span class="bold">Settings</span> > <span class="bold">Account settings</span>, then click the <span class="bold">Settings</span> tab.</li> 
 <li value="3">In the <span class="bold">Sharing</span> section, to the right of <span class="bold">Recipients can view all versions</span>, select <span class="bold">Enable</span> or <span class="bold">Disable</span> to indicate whether you want to allow&nbsp;recipients to view all versions of a <em>proof</em> within the <em>proofing viewer</em> when the Proof URL is enabled.</li> 
</ol>

## Configure *proof* visibility based on workflow stage activity

You can specify when *proofs* with an automated workflow are visible to users who are associated with a given stage.

>[!NOTE]
>
>* This option is available&nbsp;only when using the standalone *Workfront Proof* application; it is not available when using a *Workfront Proof* instance that is integrated with *Workfront* or when *proofing* within *Workfront*.
>
>* Users receive an email notification about the *proof* only after it enters the stage the user is associated with, regardless of this setting.
>

To configure when *proofs* with an automated workflow are visible to users:

<ol> 
 <li value="1"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     From 
    <em>Workfront</em>, click the Main Menu 
    <img src="assets/main-menu-icon.png">, then click Proofing 
    <img src="assets/proofing-in-main-menu.png"> to access 
    <em>Workfront Proof</em>. 
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    From 
   <em>Workfront</em>, click the Main Menu 
   <img src="assets/main-menu-icon.png">, then click Proofing 
   <img src="assets/proofing-in-main-menu.png"> to access 
   <em>Workfront Proof</em>. 
  </MadCap:conditionalText> <br> </li> 
 <li value="2">Click <span class="bold">Settings</span> > <span class="bold">Account settings</span>, then click the <span class="bold">Settings</span> tab.</li> 
 <li value="3"> <p>In the&nbsp;<span class="bold">Sharing</span>&nbsp;section, enable or disable&nbsp;<span class="bold">Proof visibility based on stage activation</span>.</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader"><span class="bold">Disabled</span> (default)</td> 
     <td>Proofs are visible to users at the time&nbsp;the <em>proof</em> is created.<br><p>Any user associated with a stage in the workflow for the <em>proof</em> can see the <em>proof</em> in search results immediately after the <em>proof</em> is created.</p></td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Enabled</span> </td> 
     <td> <p>Proofs are visible to users only&nbsp;after the stage they are associated with becomes <span class="bold">active.</span></p> <note type="note">  
       <ul> 
        <li><em style="font-style: normal;">After you enable this option, existing <em>proofs</em> are still visible to users who could view it when it was created.</em> </li> 
        <li><em style="font-style: normal;">After a user gains access to a version of a <em>proof</em> (because the stage the user is associated with becomes active), the user can see only the version where the stage is activated. If a previous version never reached the stage the user is associated with, the user cannot see that version of the <em>proof</em>.&nbsp;</em> </li> 
       </ul> 
      </note> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
</ol>

