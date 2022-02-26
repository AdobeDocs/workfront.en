---
filename: create-and-manage-layout-templates
title: Layout Templates overview
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
title: Create and manage layout templates
description: As a Workfront administrator or a group administrator, you can create and modify layout templates to customize the following layout elements in Workfront for your users:
---

# Create and manage layout templates

<!--
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p>As a <em>Workfront administrator</em> or a <em>group administrator</em>, you can create and modify layout templates to customize the following layout elements in <em>Workfront</em> for your users: </p>
<ul>
<li>Main Menu <img src="assets/main-menu-icon.png"></li>
<li>Left navigation panel</li>
<li>Home area </li>
<li>Views, filters, and groupings people use with lists and reports.</li>
<li>On-screen terminology</li>
</ul>
<p>After you create or modify a layout template, you can assign it to individual users, teams, groups, or job roles.</p>
<p>Every user's default <em>Workfront</em> layout depends on their access level and license type. For example, some users might not see some areas in the Main Menu. For more information, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md" class="MCXref xref">About the default Adobe Workfront layout</a>.</p>
<h2>Access requirements</h2>
<p>You must have the following to perform the steps in this article:</p>
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
<td> <p>You must be a <em>Workfront administrator</em>. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <note type="note">
If you still don't have access, ask your
<em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a
<em>Workfront administrator</em> can modify your access level, see
<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.
</note> </td>
</tr>
</tbody>
</table>
<h2>Considerations for creating and managing layout templates</h2>
<ul>
<li>Users can customize a few areas of their own layout. When you change a layout template, your changes merge with any customizations they have made, without overwriting or resetting them. This is also true if you assign users to a new layout template.</li>
<li> <p>Your older layout templates created in <em>Adobe Workfront Classic</em> have been automatically available in your instance of <em>the new Adobe Workfront experience</em> since they were migrated in early Fall 2019. Layout templates created in <em>Adobe Workfront Classic</em> after that time were migrated in April 2020. We recommend that you update these layout templates in <em>the new Adobe Workfront experience</em> to take advantage of new functionality and to make them even more useful in that environment.</p> <p>If you created a layout template recently in <em>Workfront</em> Classic and want it available for your users in <em>the new Adobe Workfront experience</em>, you can migrate it there. For instructions, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/migrate-layout-templates-to-nwe.md" class="MCXref xref">Migrate your layout templates to the new Adobe Workfront experience</a>.</p> <p>Keep in mind that the migrated version and the original version of each layout template are separate because they serve two different environments, so if you edit one version, your changes don't affect the other version.</p> </li>
<li><em>Group administrators</em> and users with a Plan license who can edit other users can add system-level and group-level layout templates to the users they can manage when editing their profile.</li>
<li><em>Group administrators</em> cannot assign layout templates to job roles or teams.</li>
</ul>
<p>For more information about layout templates, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md" class="MCXref xref">Layout templates</a>.</p>
<h2>Create or modify a layout template</h2>
<ol>
<li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li>
<li value="2">In the left panel, click <span class="bold">Interface</span> > <span class="bold">Layout Templates</span>.</li>
<li value="3"> <p>Click <span class="bold">New Layout Template</span>.</p> <p>Or</p> <p>Click the name of the layout template you want to modify.</p> </li>
<li value="4">If you are creating a new layout template, type a <span class="bold">Layout template name</span> and (optional) a <span class="bold">Description</span> for it.</li>
<li value="5"> <p>Customize areas of the user interface, as described in the following articles:</p>
<ul>
<li><a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref">Customize the Main Menu using a layout template</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md" class="MCXref xref">Customize the left panel using a layout template</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md" class="MCXref xref">Customize pinned pages using a layout template</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md" class="MCXref xref">Customize the Details view using a layout template</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md" class="MCXref xref">Customize Home and Summary using a layout template</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md" class="MCXref xref">Customize the landing page using a layout template</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md" class="MCXref xref">Customize Filters, Views, and Groupings using a layout template</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md" class="MCXref xref">Customize user interface terminology using a layout template</a> </li>
</ul> </li>
<li value="6"> <p>Continue on to test your layout template and make it available to users, as described in the articles below:</p>
<ul>
<li><a href="../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md" class="MCXref xref">Testing a new layout template</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md" class="MCXref xref">Grant administrative access for a layout template</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref">Assign users to a layout template</a> </li>
</ul> </li>
</ol>
<p>You can also create a new layout template by copying it and changing the copy. For more information, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md" class="MCXref xref">Copy a layout template</a>.</p>
</div>
-->

As a *Workfront administrator* or a *group administrator*, you can create and modify layout templates to customize the following layout elements in *Workfront* for your users:

<ul> 
 <li>Main Menu <img src="assets/main-menu-icon.png"></li> 
 <li>Left navigation panel</li> 
 <li>Home area </li> 
 <li>Views, filters, and groupings people use with lists and reports.</li> 
 <li>On-screen terminology</li> 
</ul>

After you create or modify a layout template, you can assign it to individual users, teams, groups, or job roles.

Every user's default *Workfront* layout depends on their access level and license type. For example, some users might not see some areas in the Main Menu. For more information, see [About the default Adobe Workfront layout](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

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

## Considerations for creating and managing layout templates

* Users can customize a few areas of their own layout. When you change a layout template, your changes merge with any customizations they have made, without overwriting or resetting them. This is also true if you assign users to a new layout template.
* Your older layout templates created in *Adobe Workfront Classic* have been automatically available in your instance of *the new Adobe Workfront experience* since they were migrated in early Fall 2019. Layout templates created in *Adobe Workfront Classic* after that time were migrated in April 2020. We recommend that you update these layout templates in *the new Adobe Workfront experience* to take advantage of new functionality and to make them even more useful in that environment.

  If you created a layout template recently in *Workfront* Classic and want it available for your users in *the new Adobe Workfront experience*, you can migrate it there. For instructions, see [Migrate your layout templates to the new Adobe Workfront experience](../../../administration-and-setup/customize-workfront/use-layout-templates/migrate-layout-templates-to-nwe.md).

  Keep in mind that the migrated version and the original version of each layout template are separate because they serve two different environments, so if you edit one version, your changes don't affect the other version.

* *Group administrators* and users with a Plan license who can edit other users can add system-level and group-level layout templates to the users they can manage when editing their profile.
* *Group administrators* cannot assign layout templates to job roles or teams.

For more information about layout templates, see [Layout templates](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

## Create or modify a layout template

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">In the left panel, click <span class="bold">Interface</span> > <span class="bold">Layout Templates</span>.</li> 
 <li value="3"> <p>Click <span class="bold">New Layout Template</span>.</p> <p>Or</p> <p>Click the name of the layout template you want to modify.</p> </li> 
 <li value="4">If you are creating a new layout template, type a <span class="bold">Layout template name</span> and (optional) a <span class="bold">Description</span> for it.</li> 
 <li value="5"> <p>Customize areas of the user interface, as described in the following articles:</p> 
  <ul> 
   <li><a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref">Customize the Main Menu using a layout template</a> </li> 
   <li><a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md" class="MCXref xref">Customize the left panel using a layout template</a> </li> 
   <li><a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md" class="MCXref xref">Customize pinned pages using a layout template</a> </li> 
   <li><a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md" class="MCXref xref">Customize the Details view using a layout template</a> </li> 
   <li><a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md" class="MCXref xref">Customize Home and Summary using a layout template</a> </li> 
   <li><a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md" class="MCXref xref">Customize the landing page using a layout template</a> </li> 
   <li><a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md" class="MCXref xref">Customize Filters, Views, and Groupings using a layout template</a> </li> 
   <li><a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md" class="MCXref xref">Customize user interface terminology using a layout template</a> </li> 
  </ul> </li> 
 <li value="6"> <p>Continue on to test your layout template and make it available to users, as described in the articles below:</p> 
  <ul> 
   <li><a href="../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md" class="MCXref xref">Testing a new layout template</a> </li> 
   <li><a href="../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md" class="MCXref xref">Grant administrative access for a layout template</a> </li> 
   <li><a href="../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref">Assign users to a layout template</a> </li> 
  </ul> </li> 
</ol>

You can also create a new layout template by copying it and changing the copy. For more information, see [Copy a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md).
