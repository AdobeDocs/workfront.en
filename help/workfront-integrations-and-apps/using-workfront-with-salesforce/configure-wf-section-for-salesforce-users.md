---
filename: configure-wf-section-for-salesforce-users
product-area: workfront-integrations;setup;user-management
navigation-topic: workfront-for-salesforce
title: Configure the Adobe Workfront section for Salesforce users
description: A Pro Workfront Plan is required to use this feature. For more information about the various plans available, see Workfront Plans.
---

# Configure the *Adobe Workfront* section for Salesforce users

A Pro *Workfront* Plan is required to use this feature. For more information about the various plans available, see [*Workfront* Plans.](https://www.workfront.com/plans)

After you install *Adobe Workfront* for Salesforce as a *Workfront administrator*, you can make it available to your users by adding it in a new section to their Opportunity and Account page layouts in Salesforce.&nbsp;

For information about installing *Workfront* for Salesforce, see [Install Adobe Workfront for Salesforce](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

For users to have *Workfront* available in both the Classic and Lightening Experience frameworks, you must add the WorkfrontOpportunities and the WorkfrontAccounts Visualforce pages to the Opportunity and Accounts page layouts, respectively.

## Access requirements

You must have the following access to use the functionality described in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p>Plan</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <p>[Insert any access level configurations needed] <draft-comment>
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Example: Edit access to Documents
       </MadCap:conditionalText>
      </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       Example: Edit access to Documents
      </MadCap:conditionalText></p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> <draft-comment>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront administrator</em>. For information on <em>Workfront administrators</em>, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p>
     </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront administrator</em>. For information on <em>Workfront administrators</em>, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <draft-comment>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>group administrator</em>. For more information on <em>group administrators</em>, see <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a>.</p>
     </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>group administrator</em>. For more information on <em>group administrators</em>, see <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a>.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>[Insert any access level configurations needed] <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
      Example: Edit access to Documents
     </MadCap:conditionalText></p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront administrator</em>. For information on <em>Workfront administrators</em>, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>group administrator</em>. For more information on <em>group administrators</em>, see <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a>.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>[Insert permissions needed and specify the object] <draft-comment>
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Example: View access or higher on Documents
       </MadCap:conditionalText>
      </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       Example: View access or higher on Documents
      </MadCap:conditionalText></p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[Insert permissions needed and specify the object] <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
      Example: View access or higher on Documents
     </MadCap:conditionalText></p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Prerequisites

* You must have a Salesforce instance with access to a system administrator account.
* You must have a *Workfront* instance with access to a system administrator account.

## Configure the *Workfront* section in the Salesforce Classic framework

<ol> 
 <li value="1"> Log in to Salesforce as a <em>Workfront administrator</em>.</li> 
 <li value="2"> Click <span class="bold">Setup.</span></li> 
 <li value="3">In the <span class="bold">Build</span> section, expand <span class="bold">Customize.</span></li> 
 <li value="4"> <p>Expand <span class="bold">Opportunities</span>, then click <span class="bold">Page Layouts&nbsp;</span>to add the <em>Workfront</em> section to an <span class="bold">Opportunity</span>.<br></p> <p>Or<br></p> <p>Expand <span class="bold">Accounts</span>, then click <span class="bold">Page Layouts&nbsp;</span>to add the <em>Workfront</em> section to an Account.</p> </li> 
 <li value="5"> <p>Click <span class="bold">Edit</span> on an existing layout.<br></p> <p>Or<br></p> <p>Click <span class="bold">New</span> to add a new layout.&nbsp;</p> </li> 
 <li value="6">(Optional) Drag the <span class="bold">Section</span> component to the layout and drop it in the desired position.<br><img src="assets/salesforce-new-section-properties-350x210.png" alt="salesforce_new_section_properties.png" style="width: 350;height: 210;"><br></li> 
 <li value="7"> <p>(Optional) Specify a name for the new section.<br></p> <p>We recommend that you name this section <span class="bold"><em>Workfront</em></span>.</p> </li> 
 <li value="8"> <p>(Optional) Specify the desired <span class="bold">Layout</span> and <span class="bold">Tab-key Order </span>for the new section.<br></p> <p>We recommend that you select&nbsp;<span class="bold">1-Column</span> layout for the <em>Workfront</em> section.&nbsp;</p> </li> 
 <li value="9">Click <span class="bold">OK</span>.</li> 
 <li value="10">In the <span class="bold">Layout</span> area, click <span class="bold">Visualforce Pages.</span></li> 
 <li value="11"> <p>Drag and drop the <span class="bold">WorfrontOpportunities</span> component to the new section in the&nbsp;<span class="bold">Opportunities</span>&nbsp;<span class="bold">Layout</span>.<br></p> <p>Or<br></p> <p>Drag and drop the <span class="bold">WorkfrontAccounts</span> component to the new section in the&nbsp;<span class="bold">Account</span>&nbsp;<span class="bold">Layout</span>.<br><img src="assets/workfrontaccounts-component-350x139.png" alt="WorkfrontAccounts_component.png" style="width: 350;height: 139;"></p> </li> 
 <li value="12">Click the <span class="bold">Properties</span> icon in the upper right of the newly added component.<br><img src="assets/salesforce-visualforce-page-properties-350x174.png" style="width: 350;height: 174;"><br></li> 
 <li value="13">To achieve an optimal display, specify the following properties for the <em>Workfront</em> Visualforce page: 
  <ul>
   <li><span class="bold">Width (in pixels or %)</span>: 100%</li>
   <li><span class="bold">Height (in pixels)</span>: 600</li>
   <li>Select <span class="bold">Show scrollbars</span>.</li>
  </ul></li> 
 <li value="14">Click <span class="bold">OK</span>.&nbsp;</li> 
 <li value="15"> <p>Click <span class="bold">Save</span> to save your layout.</p> <p>All users who have this layout assigned to them are now able to see the <em>Workfront</em> section on their Opportunities or Accounts objects.</p> <p> Users see a <em>Workfront</em> login screen on the <em>Workfront</em> section. If they do not have a <em>Workfront</em> account, they can collapse the section, but not remove it from their layout.&nbsp;</p> <p> <img src="assets/salesforce-classic-opportunity-with-workfront-panel-350x161.png" alt="salesforce_classic_opportunity_with_workfront_panel.png" style="width: 350;height: 161;"> <br> </p> </li> 
</ol>

## Configure the *Workfront* section in the Salesforce Lightning Experience framework

You can add the *Workfront* section to the layout of a Salesforce Opportunity or Account in the Salesforce Lightning Experience framework either by accessing the Setup area, or from an Account or Opportunity object.&nbsp;

* [Configure the Workfront section at the Setup level](#lightning-setup-level) 
* [Configure the Workfront Section at the Opportunity or Account level](#lighting-account-opportunity-level)

### Configure the *Workfront* section at the Setup level

1. Log into Salesforce as a system administrator.&nbsp; 
1. Click the `Setup` icon, then click `Setup`. 

1. Expand `Object and Fields`, then click `Object Manager`. 

1. Click `Opportunity`to customize the layout of an Opportunity.

   Or

   Click `Account`to customize the layout of an Account. 

1. Click `Page Layouts`. 
1. Click the name of an existing page layout to edit it.

   Or

   Click `New` to create a new page layout. 

1. Continue with [Configure the Workfront Section at the Opportunity or Account level](#lighting-account-opportunity-level) below.

### Configure the *Workfront* Section at the Opportunity or Account level

<ol> 
 <li value="1"> Log in to Salesforce as a system administrator.&nbsp; </li> 
 <li value="2"> Go to an <span class="bold">Opportunity</span> or <span class="bold">Account</span>. </li> 
 <li value="3"> Click the <span class="bold">Setup</span> icon, then click <span class="bold">Edit Page</span>.<br><img src="assets/salesforce-lightning-opportunity-edit-area-350x116.png" alt="salesforce_lightning_opportunity_edit_area.png" style="width: 350;height: 116;"><br></li> 
 <li value="4"> Expand the <span class="bold">Custom-Managed</span> section. </li> 
 <li value="5"> <p> Drag and drop the <span class="bold"><em>Workfront</em></span> component on your Opportunity or Account page.<br></p> <p>We recommend using the full width of the page for the <em>Workfront</em> section instead of one of the columns of the layout.</p> <p> <img src="assets/salesforce-lightning-builder-350x229.png" alt="salesforce_lightning_builder.png" style="width: 350;height: 229;"> </p> </li> 
 <li value="6"> <p>Click <span class="bold">Save</span>.</p> <p>All users who have this layout assigned to them are now able to see the <em>Workfront</em> section on their Opportunities or Accounts objects.</p> <note type="note">
   Users see a 
   <em>Workfront</em> login screen on the 
   <em>Workfront</em> section. If they do not have a 
   <em>Workfront</em> account, they can collapse the section, but not remove it from their layout. Users can log in using the authentication method you have enabled: Enhanced Authentication or your Security Assertion Markup Language (SAML) URL.
  </note> <p> <img src="assets/salesforce-lightning--workfront-panel-350x127.png" alt="salesforce_lightning__workfront_panel.png" style="width: 350;height: 127;"> </p> </li> 
</ol>

