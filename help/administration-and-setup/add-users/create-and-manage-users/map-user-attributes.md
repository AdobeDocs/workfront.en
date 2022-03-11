---
filename: map-user-attributes
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Map user attributes and auto-provision new users
description: Using single sign-on (SSO), you can pass attributes from your identity provider’s Active Directory to your Adobe Workfront users. You can also add new users to Workfront using the Auto-Provision option (also called Just In Time Provisioning or JIT).
---

# Map user attributes and auto-provision new users

Using single sign-on (SSO), you can pass attributes from your identity provider’s Active Directory to your Adobe Workfront users. You can also add new users to Workfront using the Auto-Provision option (also called Just In Time Provisioning or JIT).

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

## Tips for mapping attributes

Keep the following in mind when mapping attributes:

* Always test in a Preview sandbox or a Customer Refresh (CR) sandbox.
* Test with both administrator and non-administrator accounts to confirm that you are mapping attributes correctly.
* Attributes are mapped every time a user signs into Workfront via SSO, not just during Auto-Provisioning.

## Map user attributes and auto-provision new users

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">Click <span class="bold">System</span> > <span class="bold">Single Sign-On (SSO)</span>.</li> 
 <li value="3">In the <span class="bold">Type</span> drop-down, click <span class="bold">SAML 2.0</span>.</li> 
 <li value="4"> <p> Click <span class="bold">Map User Attributes</span>.</p> <p> <img src="assets/map-user-attributes-350x253.png" style="width: 350;height: 253;"> </p> </li> 
 <li value="5"> <p>(Optional) If you want Workfront to create new users from your Active Directory automatically, click <span class="bold">Auto-Provision User</span>.</p> <p>This feature requires attribute mapping.</p> </li> 
 <li value="6"> <p>In the row of options that appears, map the attributes you need for your Workfront users.</p> <p>You can map attributes such as Address, Manager, Job Role, Home Group, and so on.</p> <p>Attribute mappings work on a 1:1 Ratio. For example, you cannot set every group that a user belongs to; you can set only one per user.</p> <note type="important">  
   <ul> 
    <li>The following attributes are required for each user: 
     <ul> 
      <li>First Name</li> 
      <li>Last Name</li> 
      <li>Email Address</li> 
     </ul></li> 
    <li>We do not recommend mapping Access Levels in the Attribute Mappings. If you do, be careful when you are setting the default value to make sure that you don't remove Admin Access inadvertently.</li> 
   </ul> 
  </note> <p>The following table explains the fields you can use to map attributes:</p> 
  <table cellspacing="0">   
   <tbody> 
    <tr> 
     <td role="rowheader">Workfront User Attribute</td> 
     <td>Choose the name of the attribute you are mapping</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Directory Attribute</td> 
     <td>Type the SSO attribute label you want to use.<!--
       Is this right? I’d like to explain this and “Default Value” and their relationship. I’m trying to keep new/unexperienced sysadmins in mind.
      --></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Default Value</td> 
     <td> <p>After you choose a Workfront User Attribute, if the value is NULL during the connection, this field fills in with the corresponding default value in the system. Type a value here only if you plan to apply attribute mapping rules (see step 7). The default value acts as an exception to those rules. <!--
        Is this right?
       --></p> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="7"> <p>(Optional) Click <span class="bold">Rules</span> to add a rule to the attribute.</p> 
  <ol style="list-style-type: lower-alpha;"> 
   <li value="1">In the drop-down, choose the attribute modifier you want to use.</li> 
   <li value="2"> <p>In the 2 fields to the right, type the directory attribute value and the value you want to replace it with.</p> <p> <img src="assets/rule-fields-350x64.png" style="width: 350;height: 64;"> </p> </li> 
  </ol> <p>You can click <span class="bold">Add Rule</span> to add more rules to the attribute.</p> </li> 
 <li value="8">(Optional) To map more user attributes, click <span class="bold">Add Mapping</span> and repeat steps 6-7.</li> 
 <li value="9">Click <span class="bold">Save</span>.</li> 
</ol>

