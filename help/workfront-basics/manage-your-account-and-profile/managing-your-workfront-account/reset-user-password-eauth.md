---
filename: reset-user-password-eauth
product-area: user-management
navigation-topic: manage-your-workfront-account
title: Reset a user's password with Enhanced Authentication
description: When Enhanced Authentication (eAuth) is enabled for your Workfront Environment, a Workfront administrator can’t reset login credentials for another user. This differs from Workfront environments without eAuth or those environments for which Single Sign On (SSO) is enabled.
---

# Reset a user's password with Enhanced Authentication

When Enhanced Authentication (eAuth) is enabled for your Workfront Environment, a *Workfront administrator* can’t reset login credentials for another user. This differs from Workfront environments without eAuth or those environments for which Single Sign On (SSO) is enabled.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan</td> 
   <td> <p> Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>System administrator </p> </td> 
  </tr> 
 </tbody> 
</table>

## Reset a user’s password in an eAuth enabled environment

<ol> 
 <li value="1"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click the 
    <span class="bold">Main Menu</span> icon 
    <img src="assets/main-menu-icon.png"> in the upper-right corner of 
    <em>Workfront</em>, then click 
    <span class="bold">Users</span> 
    <img src="assets/users-icon-in-main-menu.png">. 
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Click the 
   <span class="bold">Main Menu</span> icon 
   <img src="assets/main-menu-icon.png"> in the upper-right corner of 
   <em>Workfront</em>, then click 
   <span class="bold">Users</span> 
   <img src="assets/users-icon-in-main-menu.png">. 
  </MadCap:conditionalText></li> 
 <p> <draft-comment>
   <img src="assets/main-menu-users-highlighted-nwe-350x456.png" style="width: 350;height: 456;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
  </draft-comment><img src="assets/main-menu-users-highlighted-nwe-350x456.png" style="width: 350;height: 456;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> 
 <li value="2"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Select the 
    <span class="bold">User</span> that requires a password reset.
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Select the 
   <span class="bold">User</span> that requires a password reset.
  </MadCap:conditionalText></li> 
 <p> <img src="assets/100520classicnweselectuser-350x105.png" style="width: 350;height: 105;"> </p> 
 <li value="3">Click the <span class="bold">More button</span> that appears after you've chosen the desired <span class="bold">User</span> and select the <span class="bold">Send Forgot Password Email</span> option from the drop-down menu.</li> 
 <p> <img src="assets/100520classicnwesendemail-350x134.png" style="width: 350;height: 134;"> </p> 
</ol>

After selecting the `Send Forgot Password Email` option, an email is sent to the selected user that contains instructions for them to change their own password.

![](assets/pwresetemail-resized-350x461.png)

