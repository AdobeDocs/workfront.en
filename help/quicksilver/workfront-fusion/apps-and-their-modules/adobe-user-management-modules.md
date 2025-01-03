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

## Prerequisites

## Create a connection to Adobe User Management

## Adobe User Management modules and their fields

When you configure Adobe User Management modules, Workfront Fusion displays the fields listed below. Along with these, additional Adobe User Management fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Searches

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

#### Add a user as a member of a group

#### Create a new user

#### Remove the membership of a user from groups

#### Update an existing user

### User group actions

#### Add memberships for a user group

#### Create a user group

#### Delete an existing user group

#### Remove memberships for a user group

#### Update an existing user group

### Other

#### Make a custom API call










