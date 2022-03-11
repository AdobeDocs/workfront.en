---
filename: router-module
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Router module
description: The Router module allows you to branch your flow into several routes and process the data within each route differently. Once a Router module receives a bundle, it forwards it to each connected route in the order the routes were attached to the Router module.
---

# Router module

The Router module allows you to branch your flow into several routes and process the data within each route differently. Once a Router module receives a bundle, it forwards it to each connected route in the order the routes were attached to the Router module.

>[!NOTE]
>
>* To verify the order of the routes, you can click the Auto-align icon, which will arrange the routes according to the order from top to bottom.
>
>  To change the order, just remove the Router module and re-connect the routes in the desired order.
>
>* Routes are processed sequentially, not in parallel. A bundle is not sent to the next route until it has been completely processed by the previous route.
>

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p><span>Pro</span> or higher</p> </td> 
  </tr> Adobe Workfront license* Plan, Work 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront Fusion</span> license**</td> 
   <td> <p><span>Workfront Fusion for Work Automation and Integration</span> </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase <span>Adobe Workfront Fusion</span> as well as <span>Adobe Workfront</span> to use functionality described in this article.</td> 
  </tr> <!--
   Access level configurations* You must be a Workfront Fusion administrator for your organization. You must be a Workfront Fusion administrator for your team.
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

&#42;&#42;For information on `Adobe Workfront Fusion` licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Adding a Router module to a scenario

A Router can be added to a scenario in one of the following ways:

<ul> 
 <li> <p>If you want to connect the Router module after a module, click on the module's right handle, start typing <span class="bold">router</span> to search for it, then choose <span class="bold">Flow Control</span> > <span class="bold">Router</span> in the list of modules that displays.</p> <p> <img src="assets/connect-the-router-350x108.png" style="width: 350;height: 108;"> </p> </li> 
 <li> <p>If you want to insert the Router module between two modules, click on the wrench icon below the route connecting the two modules (or right-click the route) and choose <span class="bold">Add a router</span> from the menu.</p> <p> <img src="assets/insert-router-350x191.png" style="width: 350;height: 191;"> </p> </li> 
 <li> <p>You can insert a Router module automatically. For example, in the image below, to connect the module in the lower-right corner to the one in the upper-left corner (which is already connected to the one in the upper-right corner), drag the left handle of the lower-right module and drop it onto the upper-left module.</p> <p> <img src="assets/insert-router-automatically-350x379.png" style="width: 350;height: 379;"> </p> </li> 
</ul>

## Filters

To place a filter on a route after the Router module to filter bundles as on any other route:

<ol> 
 <li value="1"> <p>Click one of the dots in the route.</p> <p> <img src="assets/router-click-a-dot-in-route-350x339.png" style="width: 350;height: 339;"> </p> </li> 
 <li value="2">In the <span class="bold">Set up a filter</span> box that displays, add conditions, then click <span class="bold">OK</span> to save the filter setup.</li> 
</ol>

![](assets/set-up-a-filter-2-350x242.png)

For more information, see [Add a filter to a scenario](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

## The fallback route

The filter setup on a route after a Router module contains a special option: The fallback route:

![](assets/fallback-route-350x260.png)

When enabled, this route is used in the case when a bundle cannot continue on from the Router module via any other route because the filters on the other routes filtered it out.

The Fallback route is distinguished with a different arrow sign inside the Router module:

![](assets/arrow-sign-in-router-module-350x361.png)

## If/Else

A typical use case of the fallback route is to continue the flow with one route if the condition is met and with another route if it is not, as in the following steps:

<ol> 
 <li value="1"> <p>Insert a Router module in your scenario.</p> </li> 
 <li value="2">Connect both routes to the Router module .</li> 
 <li value="3"> <p>Click on the first route and specify a condition:</p> <p> <img src="assets/set-up-a-filter-2-350x242.png" style="width: 350;height: 242;"> </p> </li> 
 <li value="4"> <p>Click on the second route and enable the fallback route option:</p> <p> <img src="assets/enable-fallback-route-option-350x238.png" style="width: 350;height: 238;"> </p> </li> 
</ol>

