

# Grant access to teams

As an *Adobe Workfront administrator*, you can use an access level to define a user’s access to teams in *Workfront*, as explained in [Access levels overview](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

>[!NOTE]
>
>This functionality, releasing with 2022.1, does not change your users' existing access to teams. For more information, see [How users' existing access to teams remains unchanged in the 2022.1 Teams access level setting](#the) in this article.

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
   <td> <p>You must be a <em>Workfront administrator</em>. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configure users’ access to edit users using a custom access level

<ol> 
 <li value="1">Begin creating or editing the access level, as explained in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Create or modify custom access levels</a>.</li> 
 <li value="2">Click the gear icon <img src="assets/gear-icon-settings.png"> on the <span class="bold">View</span> or <span class="bold">Edit</span> button to the right of <em>Teams</em>, then select the abilities you want to grant under <b>Fine-tune your settings</b>.
  <ol>
   <li value="1"><p><b>View</b>: If you are configuring how users with any license can view teams, change any of the following options:</p>
    <table cellspacing="0">
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
    </table></li>
   <li value="2"><p><b>Edit</b>: If you are configuring how users with a <em>Plan</em> license and <em>Work</em> license can manage teams, change any of the following options:</p>
    <table cellspacing="0">
     <col>
     <col>
     <tbody>
      <tr>
       <td role="rowheader"><span class="bold">Create</span></td>
       <td><p>Allows users with a <em>Plan</em> license or <em>Work</em> license to create teams.</p><p>This option is enabled by default.</p></td>
      </tr>
      <tr>
       <td role="rowheader"><span class="bold">Delete</span></td>
       <td><p> Allows users with a <em>Plan</em> license to delete the teams that they have access to edit (unavailable for users with a <em>Work</em> license).</p><p>This option is enabled by default.</p></td>
      </tr>
      <tr>
       <td role="rowheader"><span class="bold">Edit teams in groups I manage (Group Admins only)</span></td>
       <td><p>Allows <em>Plan</em> license users who are designated as <em>group administrators</em> to edit teams associated with the groups they manage.</p><p>This option is enabled by default.</p></td>
      </tr>
      <tr>
       <td role="rowheader"><span class="bold">Edit teams I'm on</span></td>
       <td><p>Allows users <em>Plan</em> license or <em>Work</em> license to edit teams where they are a member.</p><p>This option is disabled by default.</p></td>
      </tr>
      <tr>
       <td role="rowheader">View teams associated with my groups</td>
       <td>
        <ul>
         <li><p>Enabled: When users<draft-comment>
            <MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
              with a 
             <em>Plan</em> license or 
             <em>Work</em> license
            </MadCap:conditionalText>
           </draft-comment><MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
             with a 
            <em>Plan</em> license or 
            <em>Work</em> license
           </MadCap:conditionalText> look for teams in a Team type-ahead field, the users can see the teams associated with their groups whether or not they are team members. </p></li>
         <li><p>Disabled: When users<draft-comment>
            <MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
              with a 
             <em>Plan</em> license or 
             <em>Work</em> license
            </MadCap:conditionalText>
           </draft-comment><MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
             with a 
            <em>Plan</em> license or 
            <em>Work</em> license
           </MadCap:conditionalText> look for teams in a Team type-ahead field, the users can see the teams associated with their groups only where they are team members</p><draft-comment>
           <p data-mc-conditions="SnippetConditions.HIDE">Also, when this option is disabled, <b>View all teams</b> is automatically disabled along with it.</p>
          </draft-comment><p data-mc-conditions="SnippetConditions.HIDE">Also, when this option is disabled, <b>View all teams</b> is automatically disabled along with it.</p><p>This option is enabled by default.</p></li>
        </ul></td>
      </tr>
      <tr>
       <td role="rowheader">View all teams</td>
       <td><p>When this option is enabled and users look for teams in a Team type-ahead field, the users can see and select any team.</p><draft-comment>
         <p data-mc-conditions="SnippetConditions.HIDE">Also, when it is enabled, <b>View teams associated with my groups</b> is automatically enabled along with it. </p>
        </draft-comment><p data-mc-conditions="SnippetConditions.HIDE">Also, when it is enabled, <b>View teams associated with my groups</b> is automatically enabled along with it. </p><p>This option is enabled by default. </p></td>
      </tr>
     </tbody>
    </table></li>
  </ol></li> 
 <li value="3"> <p>Click the X to close the <span class="bold">Fine-tune your settings</span> box.</p> </li> 
 <li value="4"> <p>(Optional) To configure access settings for other objects and areas in the access level you are working on, continue with one of the articles listed in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref" data-mc-variable-override="">Configure access to Adobe Workfront</a>, such as <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref" data-mc-variable-override="">Grant access to tasks</a> and <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref" data-mc-variable-override="">Grant access to financial data</a>.</p> </li> 
 <li value="5">When you are finished, click <draft-comment>
   <b data-mc-conditions="QuicksilverOrClassic.Quicksilver">Save</b>
  </draft-comment><b data-mc-conditions="QuicksilverOrClassic.Quicksilver">Save</b>.</li> 
</ol>

>[!NOTE]
>
>* The following are true, regardless of access level settings:
>
>  * Team owners can always view and edit their teams
>  * Users always have access to view the teams they’re on
>
>* The configuration of any option available for both View and Edit (such as "View teams associated with my groups") is retained if you decide to select View instead of Edit or Edit instead of View in an access level.
>

## Access to teams by license type

For information about what users in each access level can do with issues, see the section [Teams](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#teams) in the article [Functionality available for each object type](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## How users' existing access to teams remains unchanged in the 2022.1 Teams access level setting

In an access level, when you click the gear icon ![](assets/gear-icon-in-access-levels.png) on the View or Edit button for the new Teams setting, the options "View all teams" and "View teams associated with my groups," are:

* Disabled if "View only companies, groups & teams they belong to" was enabled previously under "Set additional restrictions." 
* Enabled if "View only companies, groups & teams they belong to" was *not* enabled previously under "Set additional restrictions."

` `**Tip: **`` To view the restriction "View only companies, groups & teams they belong to," click **Set additional restrictions** at the bottom of the Edit Access Level box.

With the addition of the Teams feature in access levels, this restriction is renamed "View only companies & groups they belong to."
