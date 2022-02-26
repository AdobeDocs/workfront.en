---
filename: disable-public-proofs
content-type: tips-tricks-troubleshooting
product-area: documents
keywords: disable,public,sharing,proof,public,url
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Disable sharing proof via public URL or embed code
description: You can turn off the ability to share a proof with a public URL or embed code on a proof by proof basis or for individual users.
---

# Disable sharing proof via public URL or embed code

You can turn off the ability to share a proof with a public URL or embed code on a proof by proof basis or for individual users.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Current plan: Pro or Higher</p> <p>or</p> <p>Legacy plan: Select or Premium</p> <p>For more information about proofing access with the different plans, see <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Access to proofing functionality in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p>Current plan: <em>Work</em> or <em>Plan</em></p> <p>Legacy plan: Any (You must have proofing enabled for the user)</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader"><em>Proof Permission Profile</em> </td> 
    <td>Manager or higher</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader"><em>Proof Permission Profile</em> </td> 
   <td>Manager or higher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Documents</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or *Proof Permission Profile* you have, contact your *Workfront* or *Workfront Proof administrator*.

## Disable per *Proof*

You must be the *proof* owner or creator, or you must have the Author or Moderator proof role.

<ol> 
 <li value="1"> <p>In the project that contains the proof, click <span class="bold">Documents</span> <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     in the left panel
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    in the left panel
   </MadCap:conditionalText>.</p> </li> 
 <li value="2"> <p>Hover over the proof and select<draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
     <span class="bold">Document Details</span>
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
    <span class="bold">Document Details</span>
   </MadCap:conditionalText> .</p> </li> <draft-comment>
  <li value="3" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>In the left panel, click <span class="bold">Proofing Viewer Settings</span>, then disable the <span class="bold">Allow sharing proof via public URL or embed code</span> checkbox.</p> <p> <img src="assets/proofing-viewer-settings-350x200.png" style="width: 350;height: 200;"> </p> </li>
 </draft-comment>
 <li value="3" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>In the left panel, click <span class="bold">Proofing Viewer Settings</span>, then disable the <span class="bold">Allow sharing proof via public URL or embed code</span> checkbox.</p> <p> <img src="assets/proofing-viewer-settings-350x200.png" style="width: 350;height: 200;"> </p> </li> <draft-comment>
  <li value="4" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Click <span class="bold">Save</span>. </p> </li>
 </draft-comment>
 <li value="4" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Click <span class="bold">Save</span>. </p> </li> 
</ol>

## Disable per user

You can disable the Public proof setting for individual users in your Workfront instance. You must have a *Proof Permission Profile* of administrator to make this change.

<ol> 
 <li value="1"> <p> Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Proofing</span>.</p> </li> 
 <li value="2"> <p>Click <span class="bold">Account Settings</span> near the top-right corner.</p> </li> 
 <li value="3"> <p>Click the <span class="bold">Users</span> tab, then click on the name of a user.</p> </li> 
 <li value="4"> <p>In the <span class="bold">Default proof settings</span> section, disable the <span class="bold">Public Sharing</span> checkbox. <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
     The Allow proof option will be disabled on all new proofs generated by the user moving forward?
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
    The Allow proof option will be disabled on all new proofs generated by the user moving forward?
   </MadCap:conditionalText></p> <p> <img src="assets/default-proof-settings--public-sharing-350x210.png" style="width: 350;height: 210;"> </p> </li> 
</ol>

