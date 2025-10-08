---
title: Access Requirements in Workfront Documentation
content-type: reference
product-area: system-administration
keywords: access,level,system,administrator,planner,worker,reviewer,requestor,external,user
navigation-topic: access-levels
description: Workfront documentation how-to articles contain a table that explains the access and permissions needed for that procedure. This article explains the access requirements table in more detail and contains links for more information.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 39ea0d53-ec31-4644-b772-cfe260b8e013
---
# Access requirements in Workfront documentation

Workfront documentation how-to articles contain a table that explains the access and permissions requirements needed for that procedure. This Access requirements table allows you to understand whether you can perform a certain action in Workfront, or why you might not be able to. This article explains each element of the Access requirements table, and provides troubleshooting tips and links to more in-depth information.

If a row is absent from the Access requirements table in a given article, there are no requirements of that type for that action.

Some rows contain information labeled "New" and "Current." This is because Workfront is transitioning to a new pricing and packaging model, with some organizations operating under the new model and others still using the current model. To find out which model your organization uses, contact your Workfront administrator. You can find details and links to information in the [The Access requirements table](#the-access-requirements-table) section of this article. 

>[!NOTE]
>
>If you have questions about how any of the fields in this table apply to you, contact your Workfront administrator.

## The Access requirements table

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> Adobe Workfront packages refer to the set of features that your organization has purchased. Most Workfront functionality is available in all packages, with a few exceptions, mostly related to strategic planning and enterprise controls. <p>Packages that existed prior to 2023 are not listed.</p>
   <ul><li>To find out what Adobe Workfront package your organization uses, including whether your organization is under the new or current packaging model, contact your Workfront administrator.</li>
   <li>For instructions on how a Workfront administrator can locate your organization's Workfront package, see <a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-package" class="MCXref xref">View your organization's cluster and Workfront package</a>.</li><li>For more information on the Workfront packages, see <a href="https://business.adobe.com/products/workfront/pricing.html">Adobe Workfront pricing and packaging</a>.</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> Adobe Workfront licenses refer to the set of Workfront features included with the license assigned to you. For example, one user might have a license that includes marking work items complete and logging time, while another user has a license that allows them only to approve assets or submit requests. <p> 
   <ul>
   <li>To find out which license you are assigned, contact your Workfront administrator.</li>
   <li>For information about licenses see:
   <ul>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">New licenses overview</a></li>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Licenses overview</a></li></ul></li>
   <li>If you have the correct access level and still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-package" class="MCXref xref">Create or modify custom access levels</a>.
   </ul>
      </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Workfront offers a variety of products, and works closely with some other products on the Adobe Experience Cloud. Depending on the Workfront package that your organization purchased, you may or may not have access to these products.
   <p>For example Workfront Fusion is included in the Workfront Automation and integration package and the Workfront Ultimate package, and is available for purchase for organizations on Workfront Select or Prime plans. Workfront Planning is another product that may or may not be available based on your Workfront package.</p>
   <p>Because Workfront works closely with other Adobe products, some procedures in Workfront interact with those products directly. To follow those procedures, your organization must have purchased that product. For example, to use functionality that allows Workfront to interact with Adobe Exerience Manager Assets, your organization must have purchased Adobe Experience Manager Assets.</p>
   <p>Articles that describe procedures performed with additional products list the required product in the Product line of this table.</p>
   <p>To find out if your organization has purchased one of these additional products, contact your Workfront administrator.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> Access levels are sets of permissions for actions you can perform in Workfront, set by your Workfront administrator. <p>Workfront has built-in access levels that correspond to Workfront licenses, but your Workfront administrator can create more access levels to more accurately reflect permission sets needed in your organization.</p>
   <ul>
    <li>For information about access levels, see:
   <ul>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md" class="MCXref xref">New access levels overview</a></li>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref">Access levels overview</a></li></ul></li>
    <li>To find out the details of your access level, contact your Workfront administrator</li>
    <li>If you are a Workfront administrator, see <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configure access to Adobe Workfront</a> to learn more about granting access to specific objects in the access level.</li>  
   <li>If you have the correct access level and still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</li>
    </td>
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td><p>Object permissions refer to the access you have to individual Workfront objects when you create them or when they are shared with you. For example, you must have View access to a specific project to view the project, even if your access level allows you to view projects. This section of the Access requirement table describes any specific object permissions you need to perform the action in the article.</p>
   <p>For information on requesting additional access to an object, see <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects</a>.</p><p>For information on sharing an object, see <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md" class="MCXref xref">Share an object</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Layout template</td> 
   <td><p>Layout templates control what you can see in your Main Menu, and are configured by your Workfront administrator. This line notes any specific areas of Workfront that must be included in your Main Menu to perform the action.</p><p>In general, if an article instructs you to click on an area in the Main Menu, and that area is not visible in your Main Menu, contact your Workfront administrator to determine if that area can be made available to you.</p><p>
   For information on how a Workfront Administrator can configure the Main Menu, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref">Customize the Main Menu using a layout template</a>.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion license</td> 
   <td>Adobe Workfront Fusion has a separate licensing model than Workfront. 
   <ul><li>The current license model is based on the number of operations performed, and has no limitations on what actions an organization can perform. </li>
   <li>Legacy licenses are based on whether scenarios are able to connect to third-party applications, or whether the scenarios are used for Workfront automation only. </li>
   </ul>
   For information on Fusion licensing, see <a href="https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration" class="MCXref xref">Workfront Fusion licenses</a>.
   </td> 
  </tr> 
 </tbody> 
</table>
