---
filename: create-and-share-default-fvgs
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Create, edit, and share default filters, views, and groupings
description: You can create default filters, views, and groupings, then make them available to users in your organization.
---

# Create, edit, and share default filters, views, and groupings

You can create default filters, views, and groupings, then make them available to users in your organization.

When you create default filters, views, and groupings as described in this section, users who you share them with are able to leverage them when viewing their lists. Users can create their own filters, views, and groupings based on those you create, but they cannot directly change those you create.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <em>Workfront administrator</em>. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Create default filters, views, or groupings

<ol> 
 <li value="1"><![CDATA[	]]><draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click the 
    <span class="bold">Main Menu</span>
    <img src="assets/main-menu-icon.png">, then click 
    <span class="bold">Setup</span>.
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Click the 
   <span class="bold">Main Menu</span>
   <img src="assets/main-menu-icon.png">, then click 
   <span class="bold">Setup</span>.
  </MadCap:conditionalText> </li> 
 <li value="2"> <p>Do any of the following, depending on whether you are creating or editing a filter, view, or grouping:</p> 
  <ul> 
   <li>Click <span class="bold">Interface</span> > <span class="bold">Filters</span>.</li> 
   <li>Click <span class="bold">Interface ></span> <span class="bold">Views</span>.</li> 
   <li>Click <span class="bold">Interface</span> > <span class="bold">Groupings</span>.</li> 
  </ul> </li> 
 <li value="3"> <p>If you’re creating a filter, view, or grouping, click <span class="bold">New Filter</span>, <span class="bold">New View</span>, or <span class="bold">New Grouping,</span> then select the object type you want to associate the new filter, view, or grouping with.</p> <p>Or</p> <p>If you’re editing an existing filter, view, or grouping, select it, then click <span class="bold">Edit</span>.<br></p> </li> 
 <li value="4"> <p>Configure the filter, view, or grouping.</p> <p>For information about available options, see one of the following articles:</p> 
  <ul> 
   <li><a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Filters overview in Adobe Workfront</a> </li> 
   <li><a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Views overview in Adobe Workfront</a> </li> 
   <li><a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Groupings overview in Adobe Workfront</a> </li> 
  </ul> </li> 
 <li value="5"> <p>Click the <span class="bold">Save</span> option near the lower-left corner.</p> </li> 
</ol>

You can make the filter, view, or grouping available to users in your system. For more information about sharing filters, views or groupings with other users, see the section [Make filters, views, or groupings available to users](#making-default-filters-available-to-users) in this article.

## Make filters, views, or groupings available to users

These steps explain how to make filters, views, and groupings available from the Interface area in Setup. You can also do this in the List Controls area in Setup. For more information, see [Edit list controls: filters, views, and groupings](../../../administration-and-setup/manage-workfront/configure-reports/edit-list-controls-filters-views-groupings.md).

<ol> 
 <li value="1"><![CDATA[	]]><draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click the 
    <span class="bold">Main Menu</span>
    <img src="assets/main-menu-icon.png">, then click 
    <span class="bold">Setup</span>.
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Click the 
   <span class="bold">Main Menu</span>
   <img src="assets/main-menu-icon.png">, then click 
   <span class="bold">Setup</span>.
  </MadCap:conditionalText></li> 
 <li value="2">Click <span class="bold">Interface</span>, then click one of the following: <span class="bold">Filters</span>,<span class="bold"> Views</span>, or<span class="bold"> Groupings</span>.</li> 
 <li value="3">Select the filter, view, or grouping that you want to make available to users, then click <span class="bold">Share</span> to open the Filter Access, View Access, or Grouping Access form.</li> 
 <li value="4"> <p>(Conditional) To make the filter, view, or grouping available to all users in the system, click the <span class="bold">Gear</span> drop-down menu <img src="assets/gear-menu-for-sharing-items.png">, then click <span class="bold">Make this visible system-wide</span>. All users in the system can now see the filter, view, or grouping.</p> <p>Or</p> <p>Begin typing the name of specific users, teams, roles, groups, or companies to share the filter, view, or grouping with, then click the name when it appears in the drop-down list.</p> <p>For more information about sharing, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Overview of sharing permissions on objects in Adobe Workfront</a>.</p> </li> 
 <li value="5"> <p>Click <span class="bold">Save</span>.</p> <p>Users that you specified can now see the default filter, view, or grouping when viewing the object type that you associated it with.</p> </li> 
</ol>

## Delete filters, views, and groupings

>[!NOTE]
>
>You can hide the options All, Standard, and Nothing after selecting different defaults (see Step 5), but they can’t be deleted.You can delete any other option being used as a default, but you have to select a different default first.

<ol> 
 <li value="1"><![CDATA[	]]><draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click the 
    <span class="bold">Main Menu</span>
    <img src="assets/main-menu-icon.png">, then click 
    <span class="bold">Setup</span>.
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Click the 
   <span class="bold">Main Menu</span>
   <img src="assets/main-menu-icon.png">, then click 
   <span class="bold">Setup</span>.
  </MadCap:conditionalText></li> 
 <li value="2"> <p>Do any of the following, depending on whether you are deleting a filter, view, or grouping:</p> 
  <ul> 
   <li>Click <span class="bold">Interface</span> > <span class="bold">Filters</span></li> 
   <li>Click <span class="bold">Interface ></span><span class="bold">Views</span></li> 
   <li> <p>Click <span class="bold">Interface</span> > <span class="bold">Groupings</span></p> </li> 
  </ul> </li> 
 <li value="3"> <p>Select one or more items in the list, then click <span class="bold">Delete</span>.</p> </li> 
 <li value="4"> <p>See one of the following sections for detailed information about configuring a filter, view, or grouping. </p> 
  <ul> 
   <li><a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Filters overview in Adobe Workfront</a> </li> 
   <li><a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Views overview in Adobe Workfront</a> </li> 
   <li><a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Groupings overview in Adobe Workfront</a> </li> 
  </ul> </li> 
</ol>

