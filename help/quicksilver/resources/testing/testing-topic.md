

# Do what you need to here but keep it drafted always!

&nbsp;

# How access levels work

As an Adobe Workfront administrator, you can grant users access to view or edit objects by assigning them an access level. The articles below explain how access levels work.

* [Access levels overview](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md) 
* [Adobe Workfront licenses overview](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md) 
* [Built-in access levels in Adobe Workfront](../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md) 
* [How access levels and permissions work together](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) 
* [List your users’ access levels and licenses](../../administration-and-setup/add-users/access-levels-and-object-permissions/list-access-levels-and-licenses-for-your-users.md) 
* [Access to objects and areas by license type](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-to-objects-and-areas-by-license-type.md) 
* [Configurable access to functionality for each object type](../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)

## See also

* For information about how to create access levels, see [Configure access to Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md).
* For information about how users can share objects with each other, granting View and Edit permissions on those objects, see [Grant and request permissions to objects](../../workfront-basics/grant-and-request-access-to-objects/grant-and-request-access-to-objects.md).

&nbsp;

# Customize Home and Summary using a layout template in the new Adobe Workfront experience

You can use a Layout Template to configure the fields and global settings that users see when they click a task or issue. Each configuration you make using the steps below affects the Home area and the Summary panel in the same way.

For example, you could do the following to customize what users see in Home and Summary when they select a task:

* Add a custom field, hide a default field, and reorder the fields that display in the Details area

   * In Home:

     ![](assets/home-details-350x187.jpg)

   * And in Summary:

     ![](assets/summary-details-350x219.jpg)

* Show or hide the Documents section

You can also customize the fields that users see in the Home area when they click a project approval, document approval, or document version approval that is assigned to them.

For information about the Home area, see [Use the Home area](../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md). For information about the Summary panel, see [Summary overview in the new Adobe Workfront experience](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

1. Begin working on a layout template, as described in [Create and manage layout templates](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Click the down arrow ![](assets/dropdown-arrow.png) under **Customize what users see**, then click **Home****and Summary**.

1. In the list that appears on the left, click the object type (**Tasks**, **Issues**,**Projects**, **Documents**, or **Document Versions**) that you want to customize in Home and Summary.

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tasks</td> 
      <td> <p>In Home, your configuration for this setting affects the area to the right of a task when a user clicks the task.</p> <p>In a list of tasks, this setting affects the Summary panel that displays on the right side of the page when a user selects a task, then clicks the Open Summary icon <img src="assets/summary-panel-icon.png">.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Issues</td> 
      <td> <p>In Home, your configuration for this setting affects the area to the right of an issue when a user clicks the issue.</p> <p>In a list of issues, this setting affects the Summary panel that displays on the right side of the page when a user selects an issue, then clicks the Open Summary icon <img src="assets/summary-panel-icon.png">.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Projects</td> 
      <td>In Home, when a user clicks a project approval assigned to them, your configuration for this setting affects the area to the right of the approval.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documents</td> 
      <td>In Home, when a user clicks a document approval assigned to them, your configuration for this setting affects the area to the right of the approval.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Document Versions</td> 
      <td>In Home, when a user clicks an approval assigned to them for a particular version of a document, your configuration for this setting affects the area to the right of the approval.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >If a task is unassigned, the user assigned to the layout template will not see the field customizations in the Summary.

1. (Conditional) If you clicked Tasks or Issues in the previous step, click the category of task or issue that you want to customize.

   ![](assets/choose-cat-cstmz-nwe-350x240.png)

1. (Conditional) If the **Set primary action button** drop-down menu appears (it appears only if you select **Tasks** or **Issues** in the list on the left), click the primary action (**Done** or **Status**) that you want available for users in the Home area and in the Summary panel when they view a task or an issue.

   ![](assets/set-primary-action-button-dropdown-pdf-350x273.png)

1. Add ![](assets/add-item-plus-in-circle-blue.png) or hide ![](assets/close-or-hide---x.png) fields for the selected object type.

   ![](assets/lt-home-add-hide-fields-350x275.png)

1. Repeat steps 3-6 to customize Home area and the Summary panel for any other object types.
1. Click **Global settings**, near the lower left corner, then enable or disable any of the following options related to Adobe Workfront objects in Home and Summary:

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Show updates for work</td> 
      <td>Displays any updates made on a selected task or issue in Home or Summary. This includes both system updates and updates made by a user. Users can still filter out system updates, as described in <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable" class="MCXref xref">Enable or disable system updates</a> in <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Update work</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Log time against work</td> 
      <td>Displayed the Log time against work option when a task or issue is selected, allowing users to log time on work items directly from the Home and Summary areas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">View documents associated with work</td> 
      <td>Displays a Documents area in Home and Summary when a task or issue is selected, listing any documents attached to the task or issue. Users can click documents to view them in a preview window.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hide timestamp</td> 
      <td>Determine whether users see timestamps for the following date fields in Home and Summary:
       <ul>
        <li>Planned Completion Date</li>
        <li>Commit Date</li>
        <li><p>Submitted Date</p></li>
       </ul><p>Note:  When this option is enabled, work items that become past due are moved to the Late grouping in the Home Work List based on date only, not time.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Continue customizing the layout template.

   Or

   If you are finished customizing, click **Save**.

For more information about layout templates, see [Create and manage layout templates](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
