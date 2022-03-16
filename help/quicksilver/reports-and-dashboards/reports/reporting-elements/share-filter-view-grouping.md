---
filename: share-filter-view-grouping
product-area: reporting
navigation-topic: reporting-elements
title: Share a filter, view, or grouping in Adobe Workfront
description: The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.
---

# Share a filter, view, or grouping in Adobe Workfront

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.

Your Adobe Workfront administrator grants users access to view or edit objects when they assign access levels. For more information about granting access to objects, see [Create or modify custom access levels](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Along with the access level that users are granted, you can also grant them permissions to view or edit specific objects that you created or have access to share. For more information about access levels and permissions, see [How access levels and permissions work together](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

You can share filters, views, and groupings that you have access to view with other users.

When a filter, view, or grouping is shared with you, you can apply that filter, view, or grouping to your lists. Depending on the access granted to you, you might be able to modify it and share it with other users.

For information about how to create a filter, view, or grouping, see the following articles:

* [Filters overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md) 
* [Views overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md) 
* [Groupings overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to&nbsp;Filters, Views, Groupings</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions with access to share to a view, filter, or grouping</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Share a filter, view, or grouping

Sharing filters, views, or groupings in Workfront is identical.
You can share filters in select lists using the following interfaces: Standard interface Beta builder interface Sharing filters in select lists is different depending on which interface you use to share the filter from. For information about the types of filter-building interfaces, see Create or edit filters in Adobe Workfront. You can share views and groupings only in the standard interface. Sharing filters, views, and groupings using the standard interface Sharing filters and groupings using the beta builder interface Sharing filters, views, and groupings using the standard interface Sharing filters, views, and groupings in the standard interface is identical.

1. Go to a list of objects or a report.
1. (Conditional) From a list, click the Filter, View, or Grouping icon, then hover over the filter, view, or grouping you want to share, click the More icon , then Share. From a report, click the Filter, View, or Grouping drop-down menu, then select the filter, view, or grouping you want to share. 
1. (Conditional) If sharing from a report, click the `Filter`, `View`, or `Grouping` drop-down menu again, then click `Share Filter`, `Share View`, or `Share Grouping`.  
   The **Filter Access**, **View Access**, or **Grouping Access** dialog box displays.

1. Complete either of the following, depending on who you want to share with:

   `To share with individual users, teams, roles, groups, or companies:` In the provided field, begin typing the name of the user, team, role, group, or company you want to share with, then click the name when it appears in the drop-down list.  
   Repeat this process to share access with multiple users, teams, roles, groups, or companies.

   `To share with all users in the system:` Click the `Settings` icon, then click `Make this visible system-wide`.  
   Your administrator must select the Share System-wide option for this option to be available. For more information, see the articles [Create or modify custom access levels](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) and [Share reports, dashboards, and calendars in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

1. (Conditional) If you are sharing with individual users, teams, roles, groups, or companies, click the drop-down menu to define the level of access you want to grant.

   You can select from the following options:

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">View it</td> 
      <td> <p>Select this option to allow the share recipients only to use the shared Filter, View, or Grouping. When this option is selected, recipients cannot make any modifications to the shared item.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Manage it</td> 
      <td> <p>Select this option to allow the share recipients to use and modify the shared Filter, View, or Grouping.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Share it</td> 
      <td> <p>Click <span class="bold">Advanced Settings</span>, then select or deselect the <span class="bold">Share</span> option, depending on whether you want the share recipients to be able to share with others.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click `Save`.

   Users with whom you shared the filter, view, or grouping can access it by clicking the `Filter`, `View`, or `Grouping` drop-down menu or iconand scrolling down to the `Shared with me` section.

Sharing filters and groupings using the beta builder interface When sharing filters and groupings from lists of projects, tasks, or issues, you can share them using the beta builder interface instead of the standard interface. The beta builder interface is not available for any other objects in Workfront. You cannot build filters or groupings in the beta builder interface when building reports. Share a filter or grouping using the beta builder interface: Go to a list of projects, tasks, or issues. Click the Filter icon or Grouping icon , then enable the Beta setting to access the beta builder. It is disabled by default. This opens the beta filter builder interface. Tip: The header of the builder interface changes to blue when you enable the beta builder. After you enable the beta builder interface, Workfront keeps it enabled for all areas where it is available. Review the following lists of filters or groupings: My filters / My groupings Filters or groupings that you built and saved yourself. Suggested Filters or groupings that the Workfront administrator adds to your list of filters or groupings, either at the system level, or in your Layout Template. Shared with me Filters or groupings that others created and shared with you or that are shared system-wide. Hover over a filter or grouping you have access to at least view and share, then click the More menu , then click Share. The Filter sharing or Grouping sharing box displays. Enable the View system wide setting. This gives anyone in Workfront permission to view the filter or grouping. Or Start typing the names of users, teams, roles, groups, or companies that you want to share with in the Give access to field. (Optional) Click the right-pointing arrow next to the name of an entity to edit their permissions to the filter or grouping, then enable either the View or Manage option. (Optional) Enable or disable the additional permissions for an entity by doing one of the following: Click View and disable the Share option. It is enabled by default. Click Manage and disable either the Share or the Delete option. They are enabled by default. Tip: Users cannot receive a higher permission than their access level. If they don't have access to Edit filters or groupings in their access level, they cannot receive permissions to manage a filter or grouping. Workfront disables the Manage option for these users and the option is dimmed. Click Share. The filter or grouping is shared with the entities you specified. The filters or groupings you shared display in the Shared with me section of the filter or grouping panel for those entities.

## Video walk-through

View the following video to learn how to share filters, views, and groupings in Adobe Workfront.

>[!NOTE]
>
>The video describes how to share a grouping. However, sharing views and filters is identical to sharing a grouping.

This video was recorded in Workfront Classic. However, the content also applies to the new Workfront experience.

[ ![](assets/video-share-reporting-elements-350x198.png)](https://workfront-video.wistia.com/medias/wj9snapqio)

<!--
Additional information
-->

<!--
See also:
-->

  <!--
  Reporting elements: filters, views, and groupings
  -->

  <!--
  Create a custom report
  -->

  <!--
  Create groupings in Adobe Workfront
  -->

  <!--
  Edit existing groupings
  -->

  <!--
  Filters overview in Adobe Workfront
  -->

  <!--
  Views overview in Adobe Workfront
  -->

  <!--
  Groupings overview in Adobe Workfront
  -->

<!--
Old content
-->

<!--
You can share Filters, Views, and Groupings with other users.
-->

<!--
When a Filter, View, or Grouping is shared with you, you can apply that Filter, View, or Grouping to your lists. Depending on the access granted to you, you might be able to modify it and share it with other users.
-->

<!--
For information about how to create a Filter, View, or Grouping, see Filters overview in Adobe Workfront Views overview in Adobe Workfront and Groupings overview in Adobe Workfront.
-->

  <!--
  Sharing a Filter, View, or Grouping
  -->

  <!--
  Viewing a Filter, View, or Grouping That Has Been Shared with You
  -->

  <!--
  Removing a Shared Filter, View, or Grouping
  -->

<!--
Sharing a Filter, View, or Grouping
-->

   <!--
   Click the Filter, View, or Grouping drop-down menu, then select the Filter, View, or Grouping you want to share.
   -->

   <!--
   Click the Filter, View, or Grouping drop-down menu again, then click Share Filter, Share View, or Share Grouping. The Filter Access, View Access, or Grouping Access dialog box is displayed.
   -->

1. 

   <!--
   Complete either of the following, depending on who you want to share with:
   -->

   <!--
   To share with individual users, teams, roles, groups, or companies: In the provided field, begin typing the name of the user, team, role, group, or company you want to share with, then click the name when it appears in the drop-down list. Repeat this process to share access with multiple users, teams, roles, groups, or companies.
   -->

   <!--
   To share with all users in the system: Click the Settings icon, then click Make this visible system-wide. Your administrator must select the Share System-wide option for this option to be available. For more information, see Create or modify custom access levels and Share reports, dashboards, and calendars in Adobe Workfront.
   -->

1. 

   <!--
   (Conditional) If you are sharing with individual users, teams, roles, groups, or companies, click the drop-down menu to define the level of access you want to grant.
   -->

   <!--
   You can select from the following options:
   -->

    <!--  
    View it: Select this option to allow the share recipients only to use the shared Filter, View, or Grouping. When this option is selected, recipients cannot make any modifications to the shared item.  
    -->

    <!--  
    Manage it: Select this option to allow the share recipients to use and modify the shared Filter, View, or Grouping.  
    -->

    <!--  
    Share: Click Advanced Settings, then select or deselect the Share option, depending on whether you want the share recipients to be able to share with others.  
    -->

1. 

   <!--
   Click Save
   -->

   <!--
   Users can access the shared Filter, View, or Grouping as described in Viewing a Filter, View, or Grouping That Has Been Shared with You.
   -->

   <!--
   Users who you share the Filter, View, or Grouping with can access the shared Filter, View, or Grouping by clicking the Filter, View, or Grouping drop-down menu and scrolling down to the Shared with me section.
   -->

