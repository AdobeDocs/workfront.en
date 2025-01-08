---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe User Management modules
description: In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that manage users in your Adobe account.
author: Becky
feature: Workfront Fusion
---
# Adobe User Management modules

In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that manage users in your Adobe account.


If you need instructions on creating a scenario, see [Create a scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to use the functionality in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] or higher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Current license requirement: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration],  [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Current product requirement: If you have the [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Adobe Workfront] plan, your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article. [!DNL Workfront Fusion] is included in the [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>Or</p>
   <p>Legacy product requirement: Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Create a connection to Adobe User Management

To create a connection for your [!DNL Adobe User Management] modules:

1. Click **[!UICONTROL Add]** next to the Connection box.
    
1. Fill in the following fields:
    
    <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
        <td role="rowheader">[!UICONTROL Connection name]</td>
        <td>
          <p>Enter a name for this connection.</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Environment]</td>
        <td>Select whether you are connecting to a production or non-production environment.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Type]</td>
        <td>Select whether you are connecting to a service account or a personal account.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Enter your [!UICONTROL Adobe] [!UICONTROL Client ID]. This can be found in the [!UICONTROL Credentials] details section of the [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Enter your [!DNL Adobe] [!UICONTROL Client Secret]. This can be found in the [!UICONTROL Credentials] details section of the [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL IMS Organization ID]</td>
        <td>Enter your [!DNL Adobe] IMS credentials. The unique identifier for an organization. This is a string of the form A495E53@AdobeOrg where the prefix before the @ is a hexadecimal number. You can find this value as part of the URL path for the organization in the Admin Console or in the adobe.io console for your User Management integration.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Additional scopes]</td>
        <td>For each additional scope you want to add, click <b>Add item</b> and enter the scope.</td>
        </tr>
      </tbody>
    </table>
    
1. Click **[!UICONTROL Continue]** to save the connection and return to the module.
    


## Adobe User Management modules and their fields

When you configure Adobe User Management modules, Workfront Fusion displays the fields listed below. Along with these, additional Adobe User Management fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Searches](#searches)
* [User actions](#user-actions)
* [User group actions](#user-group-actions)
* [Other](#other)

### Searches

* [Get user groups and product profiles](#get-user-groups-and-product-profiles)
* [Get user information](#get-user-information)
* [Get users in a user group or product profile](#get-users-in-a-user-group-or-product-profile)
* [Get users in an organization](#get-users-in-an-organization)

#### Get user groups and product profiles

This search module retrieves a list of all user groups and product profiles in your organization, along with details about the groups and profiles.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions on creating a connection to Adobe User Management, see <a href="#create-a-connection-to-adobe-user-management" class="MCXref xref" >Create a connection to Adobe User Management</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Maximum number of returned results</td> 
   <td>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</td> 
  </tr> 
 </tbody> 
</table>

#### Get user information

This search module retrieves details for a single user in the organization, identified by their email address.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions on creating a connection to Adobe User Management, see <a href="#create-a-connection-to-adobe-user-management" class="MCXref xref" >Create a connection to Adobe User Management</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Email address</td> 
   <td>Enter or map the email address of the user you want to return details for. For AdobeID, Enterprise and email-federated users this should be the full email address including domain. In all cases the parameter is case-insensitive.</td> 
  </tr> 
 </tbody> 
</table>

#### Get users in a user group or product profile

This search module retrieves a list of all users in the specified user group or product profile, along with details about the users.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions on creating a connection to Adobe User Management, see <a href="#create-a-connection-to-adobe-user-management" class="MCXref xref" >Create a connection to Adobe User Management</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Group name</td> 
   <td>The user group, product profile name or an administrative group. For an admin group, the name can be one of the fixed groups <code>_org_admin</code>, <code>_deployment_admin</code>, or <code>_support_admin</code>; or a group-specific admin group. These are identified with a prefix on the group name , such as <code>_admin_groupName</code>, <code>_product_admin_productName</code>, or <code>_developer_groupName</code>. If the group exists but the admin group does not, an empty list is returned.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Direct only</td> 
   <td>Specify whether the groups field in the returned user structure contains only those product profiles of which that user is a direct member. If false, returns all groups (user groups, product profiles, and admin groups) containing the user, regardless of whether an entitlement for a particular product profile comes directly (via user assignment) or indirectly (via a user group that contains the user being assigned to the product profile). If true, returns all user groups and admin groups containing the user, but only those product profiles to which the user has been explicitly assigned an entitlement. A user can be both a direct and an indirect member of a product profile.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Exclude groups</td> 
   <td>Specify whether the response excludes the groups array from being returned for each individual user.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Status</td> 
   <td>This option applies only to product profiles. Select active to list users that have been provisioned for the product and have an active license. Select inactive to list users who have been added to the product profile but do not have an active license. If left blank, the module returns all member users regardless of their entitlement status.
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Maximum number of returned results</td> 
   <td>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</td> 
  </tr> 
 </tbody> 
</table>

#### Get users in an organization

This search module returns all users of the organization associated with the connection.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions on creating a connection to Adobe User Management, see <a href="#create-a-connection-to-adobe-user-management" class="MCXref xref" >Create a connection to Adobe User Management</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Maximum number of returned results</td> 
   <td>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</td> 
  </tr> 
 </tbody> 
</table>

### User actions

* [Add a user as a member of a group](#add-a-user-as-a-member-of-a-group)
* [Create a user](#create-a-user)
* [Remove a user from groups](#remove-a-user-from-groups)
* [Update a user](#update-a-user)

#### Add a user as a member of a group

This action module adds a user as a member of the specified group or groups. This module can add the user to up to four groups.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions on creating a connection to Adobe User Management, see <a href="#create-a-connection-to-adobe-user-management" class="MCXref xref" >Create a connection to Adobe User Management</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">User</td> 
   <td>Enter or map the user that you want to add to the groups.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Domain</td> 
   <td>For federated IDs that are not email addresses, enter the domain the user belongs to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Groups</td> 
   <td>For each group that you want to add the user to, click <b>Add item</b> and enter or map the group. You can enter up to four groups, and must enter at least one.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Use Adobe ID</td> 
   <td>Select true to ensure that the user ID is interpreted to refer to an existing Adobe ID even if a Enterprise or Federated ID exists with the same name.</td> 
  </tr> 
 </tbody> 
</table>

#### Create a user

This action module creates a new user in the organization.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions on creating a connection to Adobe User Management, see <a href="#create-a-connection-to-adobe-user-management" class="MCXref xref" >Create a connection to Adobe User Management</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID type</td> 
   <td>Select whether you want to create a user with an Adobe ID, an Enterprise ID, or a Federated ID. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Login</td> 
   <td>If you are creating a user with a Federated ID, select the login type.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Email</td> 
   <td>Enter or map the email address for the new user.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Domain</td> 
   <td>If you are creating a user with a Federated ID with a domain-based login, enter or map the domain.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">User</td> 
   <td>If you are creating a user with a Federated ID with a domain-based login, enter or map the user that this the new user will represent.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">First name</td> 
   <td>Enter or map the first name of the user.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Last name</td> 
   <td>Enter or map the last name of the user.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Country</td> 
   <td>Enter or map the two-character ISO country code. This cannot be changed after the user is created.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Option</td> 
   <td>Select the action to take if the user already exists in the organization. If no option is selected, and the user already exists, the module returns an error.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Use Adobe ID</td> 
   <td>When true, the user ID is interpreted to refer to an existing Adobe ID even if a Enterprise or Federated ID exists with the same name.</td> 
  </tr> 
 </tbody> 
</table>

#### Remove a user from groups

This action module removes the membership of a user from the specified groups. You can remove a user from up to four groups at a time.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions on creating a connection to Adobe User Management, see <a href="#create-a-connection-to-adobe-user-management" class="MCXref xref" >Create a connection to Adobe User Management</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">User</td> 
   <td>Enter or map the user that you want to remove from the groups.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Domain</td> 
   <td>For federated IDs that are not email addresses, enter the domain the user belongs to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Groups</td> 
   <td>For each group that you want to remove the user from, click <b>Add item</b> and enter or map the group. You can enter up to four groups, and must enter at least one.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Use Adobe ID</td> 
   <td>Select true to ensure that the user ID is interpreted to refer to an existing Adobe ID even if a Enterprise or Federated ID exists with the same name.</td> 
  </tr> 
 </tbody> 
</table>



#### Update a user

This action module updates an existing user.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions on creating a connection to Adobe User Management, see <a href="#create-a-connection-to-adobe-user-management" class="MCXref xref" >Create a connection to Adobe User Management</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">User</td> 
   <td>Enter or map the ID of the user you want to update. This is the user's email address, such as <code>user@example.com</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Domain</td> 
   <td>If you are updating a user with a Federated ID that is not an email address, enter or map the domain the user belongs to in order to identify the user.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Email</td> 
   <td>Enter or map the new email address for the user.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">First name</td> 
   <td>Enter or map the first name of the user.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Last name</td> 
   <td>Enter or map the last name of the user.</td> 
  </tr> 
 </tbody> 
</table>

### User group actions

* [Add memberships for a user group](#add-memberships-for-a-user-group)
* [Create a user group](#create-a-user-group)
* [Delete a user group](#delete-a-user-group)
* [Remove memberships for a user group](#remove-memberships-for-a-user-group)
* [Update a user group](#update-a-user-group)

#### Add memberships for a user group

This action module adds users and product profiles to a user group. Users added to the user group gain entitlement to all product profiles in the user group. Adding a product profile gives entitlement to that profile to users in the user group.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions on creating a connection to Adobe User Management, see <a href="#create-a-connection-to-adobe-user-management" class="MCXref xref" >Create a connection to Adobe User Management</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Group name</td> 
   <td>Enter or map name of the group that you want to remove the users or profiles from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Users</td> 
   <td>For each user that you want to add, click <b>Add user</b> and enter the user's email address.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profiles</td> 
   <td>For each profile that you want to add to the group, click <b>Add user</b> and enter the profile name</td> 
  </tr> 
 </tbody> 
</table>

#### Create a user group

This action module creates a new user group. If a group already exists with the given name, the the module can update the existing group.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions on creating a connection to Adobe User Management, see <a href="#create-a-connection-to-adobe-user-management" class="MCXref xref" >Create a connection to Adobe User Management</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Group name</td> 
   <td>Enter or map a name for the new user group.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Description</td> 
   <td>Enter or map a description for the new user group.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Option</td> 
   <td>Select the action to take if the user group already exists in the organization. If no option is selected, and the user group already exists, the module returns an error.</td> 
  </tr> 
 </tbody> 
</table>

#### Delete a user group

This action module deletes an existing user group.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions on creating a connection to Adobe User Management, see <a href="#create-a-connection-to-adobe-user-management" class="MCXref xref" >Create a connection to Adobe User Management</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Group name</td> 
   <td>Enter or map the name of the group that you want to delete.</td> 
  </tr> 
 </tbody> 
</table>

#### Remove memberships for a user group

This action module removes users or profiles from a user group. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions on creating a connection to Adobe User Management, see <a href="#create-a-connection-to-adobe-user-management" class="MCXref xref" >Create a connection to Adobe User Management</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Group name</td> 
   <td>Enter or map name of the group that you want to remove the users or profiles from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Users</td> 
   <td>For each user that you want to remove, click <b>Add user</b> and enter the user's email address.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profiles</td> 
   <td>For each profile that you want to remove from the group, click <b>Add user</b> and enter the profile name</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Use Adobe ID</td> 
   <td>When true, the user ID is interpreted to refer to an existing Adobe ID even if an Enterprise or Federated ID exists with the same name.</td> 
  </tr> 
 </tbody> 
</table>

#### Update a user group

This action module updates an existing user group.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions on creating a connection to Adobe User Management, see <a href="#create-a-connection-to-adobe-user-management" class="MCXref xref" >Create a connection to Adobe User Management</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Original group name</td> 
   <td>Enter or map the current name of the group that you want to update.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">New group name</td> 
   <td>Enter or map the new name that you want the group to have.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Original group name</td> 
   <td>Enter or map the updated description of the group.</td> 
  </tr> 
 </tbody> 

### Other

This action module makes a custom call to the Adobe User Management API.

#### Make a custom API call

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
      <td>For instructions on creating a connection to Adobe User Management, see <a href="#create-a-connection-to-adobe-user-management" class="MCXref xref" >Create a connection to Adobe User Management</a> in this article.</td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>URL</p>
      </td>
      <td>
        <p>Enter a path relative to <code>https://usermanagement.adobe.io/v2/usermanagement/</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>Method</p>
      </td>
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">Headers</td>
      <td>
        <p>Add the headers of the request in the form of a standard JSON object.</p>
        <p>For example, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] adds authorization headers and x-api-key headers automatically.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Query String  </td>
      <td>
        <p>Enter the request query string.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Body</td>
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>










