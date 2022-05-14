

# Grant access to teams

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

As an Adobe Workfront administrator, you can use an access level to define a user’s access to teams in Workfront, as explained in [Access levels overview](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

>[!NOTE]
>
>This functionality, releasing with 2022.1, does not change your users' existing access to teams. For more information, see [How users' existing access to teams remains unchanged in the 2022.1 Teams access level setting](#how-users-existing-access-to-teams-remains-unchanged-in-the-2022-1-teams-access-level-setting) in this article.

<!--
><MadCap:conditionalText style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">>
>Remove this note and the referenced section below a few months after the functionality releases>
></MadCap:conditionalText>>
-->

## Access requirements

You must have the following access to perform the steps in this article: 

<table> 
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
   <td> <p>You must be a Workfront administrator. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configure users’ access to edit users using a custom access level

1. Begin creating or editing the access level, as explained in [Create or modify custom access levels](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Click the gear icon ![](assets/gear-icon-settings.png) on the **View** or **Edit** button to the right of Teams, then select the abilities you want to grant under **Fine-tune your settings**.

   1. **View**: If you are configuring how users with any license can view teams, change any of the following options:

      <table>
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">View teams associated with my groups</td>
         <td>
          <ul>
           <li><p>Enabled: When users look for teams in a Team type-ahead field, the users can see the teams associated with their groups whether or not they are team members. </p></li>
           <li><p>Disabled: When users look for teams in a Team type-ahead field, the users can see the teams associated with their groups only where they are team members</p><p>This option is enabled by default.</p></li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader"><b>View all teams</b></td>
         <td><p>When this option is enabled and users look for teams in a Team type-ahead field, the users can see and select any team.</p><p>This option is enabled by default. </p></td>
        </tr>
       </tbody>
      </table>

   1. **Edit**: If you are configuring how users with a Plan license and Work license can manage teams, change any of the following options:

      <table>
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader"><strong>Create</strong></td>
         <td><p>Allows users with a Plan license or Work license to create teams.</p><p>This option is enabled by default.</p></td>
        </tr>
        <tr>
         <td role="rowheader"><strong>Delete</strong></td>
         <td><p> Allows users with a Plan license to delete the teams that they have access to edit (unavailable for users with a Work license).</p><p>This option is enabled by default.</p></td>
        </tr>
        <tr>
         <td role="rowheader"><strong>Edit teams in groups I manage (Group Admins only)</strong></td>
         <td><p>Allows Plan license users who are designated as group administrators to edit teams associated with the groups they manage.</p><p>This option is enabled by default.</p></td>
        </tr>
        <tr>
         <td role="rowheader"><strong>Edit teams I'm on</strong></td>
         <td><p>Allows users Plan license or Work license to edit teams where they are a member.</p><p>This option is disabled by default.</p></td>
        </tr>
        <tr>
         <td role="rowheader">View teams associated with my groups</td>
         <td>
          <ul>
           <li><p>Enabled: When users look for teams in a Team type-ahead field, the users can see the teams associated with their groups whether or not they are team members. </p></li>
           <li><p>Disabled: When users look for teams in a Team type-ahead field, the users can see the teams associated with their groups only where they are team members</p><p>This option is enabled by default.</p></li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">View all teams</td>
         <td><p>When this option is enabled and users look for teams in a Team type-ahead field, the users can see and select any team.</p><p>This option is enabled by default. </p></td>
        </tr>
       </tbody>
      </table>

1. Click the X to close the **Fine-tune your settings** box.
1. (Optional) To configure access settings for other objects and areas in the access level you are working on, continue with one of the articles listed in [Configure access to Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), such as [Grant access to tasks](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) and [Grant access to financial data](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. When you are finished, click **Save Changes**.

>[!NOTE]
>
>* The following are true, regardless of access level settings:
>
>   * Team owners can always view and edit their teams
>   * Users always have access to view the teams they’re on
>
>* The configuration of any option available for both View and Edit (such as "View teams associated with my groups") is retained if you decide to select View instead of Edit or Edit instead of View in an access level.
>

## Access to teams by license type

For information about what users in each access level can do with issues, see the section [Teams](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#teams) in the article [Functionality available for each object type](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## How users' existing access to teams remains unchanged in the 2022.1 Teams access level setting {#how-users-existing-access-to-teams-remains-unchanged-in-the-2022-1-teams-access-level-setting}

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Remove this section a few months after the functionality releases</p>
-->

In an access level, when you click the gear icon ![](assets/gear-icon-in-access-levels.png) on the View or Edit button for the new Teams setting, the options "View all teams" and "View teams associated with my groups," are:

* Disabled if "View only companies, groups & teams they belong to" was enabled previously under "Set additional restrictions." 
* Enabled if "View only companies, groups & teams they belong to" was *not* enabled previously under "Set additional restrictions."

>[!TIP]
>
>To view the restriction "View only companies, groups & teams they belong to," click **Set additional restrictions** at the bottom of the Edit Access Level box.
>
>With the addition of the Teams feature in access levels, this restriction is renamed "View only companies & groups they belong to."

