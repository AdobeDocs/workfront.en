---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Platform-based administration differences (Adobe Workfront/Adobe Business Platform)
description: If your organization has been onboarded to the Adobe Business Platform, your users use the Adobe Business Platform to access Adobe Workfront. This means that user management is largely done through the Adobe Admin Console, and that Single Sign-On (SSO) is handled through the Adobe Business Platform rather than through Workfront. As an Adobe Workfront administrator, your administration responsibilities and procedures differ based on whether your organization has been onboarded to the Adobe Business Platform. This article lists the procedures that must be handled differently, and links to instructions for both Workfront and the Adobe Admin Console.
author: Caroline
feature: System Setup and Administration
role: Admin
---

# Platform-based administration differences (Adobe Workfront/Adobe Business Platform)

If your organization has been onboarded to the Adobe Business Platform, your users use the Adobe Business Platform to access Adobe Workfront. This means that:

* User management is largely done through the Adobe Admin Console
* Single Sign-On (SSO) is handled through the Adobe Business Platform rather than through Workfront

As an Adobe Workfront administrator, your administration responsibilities and procedures differ based on whether your organization has been onboarded to the Adobe Business Platform. This article lists the procedures that must be handled differently, and links to instructions for both Workfront and the Adobe Admin Console.

## Users

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Action</th> 
   <th>For instructions in Workfront, see</th> 
   <th>For instructions in the Adobe Admin console, see</th> 
  </tr> 
 </thead> 
 <tbody> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">View information about access levels and licenses for your users</td> 
    <td> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/list-access-levels-and-licenses-for-your-users.md" class="MCXref xref">List your users' access levels and licenses</a> </p> </li> 
     </ul> </td> 
    <td> 
     <ul> 
      <li> <p>The section "View user list" in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
     </ul> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">Grant a user admin access</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Edit user details" in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Add a user to Adobe Workfront</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Add users</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a> </p> </li> 
     <li> <p>The section "Add users" in in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Add a user to Adobe Workfront Fusion</td> 
    <td> 
     <ul> 
      <li> <p><a href="../../workfront-fusion/organizations/add-user-to-an-organization.md" class="MCXref xref">Add a user to an organization in Adobe Workfront Fusion</a> </p> </li> 
     </ul> </td> 
    <td> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a> </p> </li> 
      <li> <p>The section "Add users" in in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
     </ul> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">Deactivate a user</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Remove users" in in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Delete a user</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md" class="MCXref xref">Delete users</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Permanently delete users" in <a href="https://helpx.adobe.com/enterprise/using/manage-directory-users.html">Manage directory users</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Edit a user profile</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Edit user details" in in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bulk edit user profiles</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md" class="MCXref xref">Edit user profiles in bulk</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Edit user details" in <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">Bulk CSV upload</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Import users </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Import users</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Add users" in <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">Bulk CSV upload</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Log in as another user</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md" class="MCXref xref">Log in as another user</a> </p> </li> 
    </ul> </td> 
   <td>Not available</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Renew SAML certificate</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/manage-workfront/security/renew-wf-saml-2-certificate.md" class="MCXref xref">Renew the Adobe Workfront SAML 2.0 metadata certificate</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "The digital signature in the SAML response did not validate..." in <a href="https://helpx.adobe.com/enterprise/kb/tshoot-fed-id.html">Troubleshooting Federated ID</a></p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## SSO (Single Sign-On)

Because the Adobe Business Platform controls Single Sign-On (SSO) for users, the following actions and functionality are handled automatically through the Adobe Business Platform. If your organization has not yet been onboarded to the Adobe Business Platform, you must perform these actions in Workfront.

* [Configure Adobe Workfront with Active Directory](../../administration-and-setup/add-users/single-sign-on/configure-workfront-ad.md) 
* [Configure Adobe Workfront with Azure Active Directory](../../administration-and-setup/add-users/single-sign-on/configure-workfront-azure-ad.md) 
* [Configure Adobe Workfront with LDAP](../../administration-and-setup/add-users/single-sign-on/configure-workfront-ldap.md) 
* [Configure Adobe Workfront with SAML 1.1](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-1.1.md) 
* [Configure Adobe Workfront with SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md) 
* [Configure Adobe Workfront with SAML 2.0 using ADFS](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md) 
* [Deactivate single sign-on in Adobe Workfront](../../administration-and-setup/add-users/single-sign-on/deactivate-sso.md) 
* [Update SAML 2.0 metadata in your identity provider](../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md) 
* [Update SAML 2.0 metadata in your IDP when using enhanced authentication](../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip-eauth-.md) 
* [Update users for single sign-on](../../administration-and-setup/add-users/single-sign-on/update-users-sso.md) 
* [Configure password policies for authentication](../../administration-and-setup/manage-workfront/security/configure-password-policies-authentication.md) 
* [Configure system security preferences](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md) 
* [Set up Azure Active Directory with Enhanced Authentication](../../administration-and-setup/manage-workfront/security/set-up-azure-active-directory-enhanced-authentication.md)

&nbsp;
