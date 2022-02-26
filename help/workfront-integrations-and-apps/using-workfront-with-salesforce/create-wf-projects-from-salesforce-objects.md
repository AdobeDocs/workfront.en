---
filename: create-wf-projects-from-salesforce-objects
product-area: workfront-integrations;projects
navigation-topic: workfront-for-salesforce
title: Create Adobe Workfront projects from Salesforce objects
description: After installing Adobe Workfront for Salesforce, you can define triggers that create Workfront projects when certain criteria are met on Salesforce Opportunities and Accounts.
---

# Create *Adobe Workfront* projects from Salesforce objects

After installing *Adobe Workfront* for Salesforce, you can define triggers that create *Workfront* projects when certain criteria are met on Salesforce Opportunities and Accounts.

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

To submit a *Workfront* request from a Salesforce Opportunity or Account ensure that you have the following in your environment:

* Your *Workfront administrator* has installed *Workfront* for Salesforce.  
  For more information about installing *Workfront* for Salesforce, see [Install Adobe Workfront for Salesforce](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* Your *Workfront administrator* has added the *Workfront* section to your Opportunity and Account page layouts.  
  For more information about adding the *Workfront* section to a page layout, see [Configure the Adobe Workfront section for Salesforce users](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* You have a *Workfront* account and you can log in to it from the *Workfront* section inside your Opportunity or Account.

## Configuring the Creation of *Workfront* Projects from Salesforce

* [Understanding the Automatic Creation of Projects](#understanding-creating-projects) 
* [Configuring Triggers](#configure-triggers) 
* [Understanding Project Names](#project-names)

### Understanding the Automatic Creation of Projects

As the Salesforce system administrator, you can define triggers that can automatically create projects in *Workfront* when the following things happen in Salesforce:

* The Stage of an Opportunity is updated.
* The Type of an Account is updated.&nbsp;&nbsp;

Triggers can be configured only after you have installed *Workfront* for Salesforce.&nbsp;&nbsp;  
For information about installing *Workfront* for Salesforce, see [Install Adobe Workfront for Salesforce](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Consider the following when configuring triggers to automatically create *Workfront* projects when Salesforce items are created or updated:

* You must be a Salesforce and a *Workfront* system administrator to configure triggers.&nbsp;
* After you configure the triggers, anyone who updates the Stage of an Opportunity or the Type of an Account can trigger the creation of a *Workfront* project. This includes Salesforce users who do not have a *Workfront* account.&nbsp;

* There is no limit to how many triggers you can have.
* You cannot create multiple triggers based on the same conditions. Triggers are unique by default.
* Once the project is created it is automatically linked to the opportunity or the account where it was generated.&nbsp;Once established, this link cannot be broken.
* One opportunity or account can be linked to multiple projects in *Workfront* when a triggered condition has been met multiple times in the life of the opportunity or the account.

  For example, if you define more then one Stage for an Opportunity to trigger a Project, a project is created for every defined stage that the opportunity reaches, for the life of that opportunity. Also, if you update the Stage of an Opportunity from one defined stage to another, and then update it back to the defined stage, a second project is created for the second time you update the Stage field to the same defined stage.&nbsp;

* One project in *Workfront* can be linked only to one opportunity or one account in Salesforce at any given time, but not to both at the same time.&nbsp;

### Configuring Triggers

Once you configure the triggers, the process of creating *Workfront* projects is enabled for both Salesforce Classic or Lightning Experience frameworks.

To configure triggers in Salesforce:

<ol> 
 <li value="1">Log in to Salesforce as the system administrator.&nbsp;</li> 
 <li value="2"> <p> (Conditional) In Salesforce Classic, click <span class="bold">Setup</span>, and under the <span class="bold">Build</span> section, expand <span class="bold">Lightning Bolt</span>.</p> <p>Or</p> <p>In Salesforce Lightning Experience, click the <span class="bold">Setup icon</span>, then <span class="bold">Setup</span>, and under <span class="bold">PLATFORM TOOLS</span> expand <span class="bold">Apps</span>.</p> </li> 
 <li value="3"> <p> Click <span class="bold">Installed Packages</span>.</p> <p>Notice that the <span class="bold"><em>Workfront</em></span> package has been installed.</p> </li> 
 <li value="4">Click <span class="bold">Configure</span> next to<span class="bold"> <em>Workfront</em></span>.</li> 
 <li value="5"> <p>Log in to <em>Workfront</em> as a system administrator.</p> <p>The <span class="bold">Triggers</span> page displays.</p> <p> <img src="assets/salesforce-triggers-page-empty-350x134.png" alt="salesforce_triggers_page_empty.png" style="width: 350;height: 134;"> </p> </li> 
 <li value="6">Click <span class="bold">New Trigger</span>.&nbsp;</li> 
 <li value="7">From the <span class="bold">Salesforce Object </span>drop-down menu, select <span class="bold">Opportunity</span>.<span class="bold"><br></span>This is a required field.</li> 
 <li value="8">(Conditional) Specify the following: 
  <ol>
   <li value="1">From the <span class="bold">Stage</span> drop-down menu, select a&nbsp;<span class="bold">Stage</span>.<br>When an opportunity reaches the Stage specified here, a project is created in <em>Workfront</em>. This is a required field.</li>
   <li value="2">In the <span class="bold">Portfolio or Program</span> field, start typing the name of a Portfolio or Program where you want the project to be placed in <em>Workfront</em>, then select it when it appears in the list.<br>If you do not specify a Portfolio or a Program, the new project is created and added to the Projects I Own list of the user logged in to <em>Workfront</em> when configuring the triggers. That user is also the Project Owner for the new project.</li>
   <li value="3"><p>Start typing the name of a Template that you want to associate with the new <em>Workfront</em> project, then select it when it appears in the list.<br>This is a required field.&nbsp;</p><note type="note">
     If you have specified a Template Owner on the template that you are planning to use for this integration, that becomes the Project Owner of the new project. The new projects appear under the Projects I Own list of the user who is the owner of the new project, according to the template. 
    </note></li>
   <li value="4">(Optional) Select the <span class="bold">Create a new project for each sold product type field</span>, if you want to create a new project for every type of product that is sold under any one opportunity.&nbsp;</li>
   <li value="5"><p>(Conditional) Select a <span class="bold">Product</span> in the <span class="bold">Product</span> drop-down menu.</p><p>This is a required field.</p></li>
   <li value="6"><p>(Conditional)&nbsp;Start typing the name of a <span class="bold">Template</span> that you want to associate with the new <em>Workfront</em> project if the specified Product is on the Opportunity. Select it when it appears in the list.</p><p>This is a required field.</p><p>The project created when a new product is added to the Salesforce opportunity is placed in the same Portfolio or Program selected for the opportunity.</p><note type="important">
     The project is created only when the Stage is updated on the Opportunity. A unique project is created for each product specified when the Stage field is updated, and not as the products are added to Opportunities.
    </note></li>
  </ol></li> 
 <li value="9">(Optional) Click <span class="bold">New Trigger</span>.&nbsp;</li> 
 <li value="10">(Optional)&nbsp;From the <span class="bold">Salesforce Object </span>drop-down menu, select <span class="bold">Account</span>.</li> 
 <li value="11">This is a required field.&nbsp;</li> 
 <li value="12">(Conditional) Specify the following:&nbsp;<br>
  <ol>
   <li value="1"><p>Select a <span class="bold">Type</span> from the <span class="bold">Type</span> drop-down menu.<br>When any <span class="bold">Account</span> is designated as the <span class="bold">Type</span> specified here in Salesforce, a <span class="bold">Project</span> is created in <em>Workfront</em>.</p><p>This is a required field.&nbsp;</p></li>
   <li value="2"><p>(Optional) Start typing the name of a <span class="bold">Portfolio</span> or <span class="bold">Program</span> where you want the project to be placed in <em>Workfront</em> in the <span class="bold">Portfolio or Program</span> field, then select it when it appears in the list.</p><p>If you do not specify a Portfolio or a Program, the new project is created and added to the <span class="bold">Projects I Own</span> list of the user logged in to <em>Workfront</em> from Salesforce. The user is also the Project Owner for the new project.&nbsp;</p></li>
   <li value="3"><p>Start typing the name of a <span class="bold">Template</span> that you want to associate with the new <em>Workfront</em> project, then select it when it appears in the list.</p><p>This is a required field.&nbsp;</p><note type="note">
     If you have specified a Template Owner on the template that you are planning to use for this integration, that becomes the Project Owner of the new project. The new projects appear under the 
     <span class="bold">Projects I Own</span> list of the user who is the owner of the new project, according to the template. 
    </note></li>
  </ol><img src="assets/salesforce-triggers-page-with-cleaned-up-template-names-350x157.png" alt="salesforce_triggers_page_with_cleaned_up_template_names.png" style="width: 350;height: 157;"></li> 
 <li value="13">Click <span class="bold">Save</span>.<br><em>Workfront</em> projects are now generated every time any of the triggers are met.</li> 
</ol>

### Understanding Project Names

Depending on which trigger generated the projects, the names of the projects in *Workfront* could follow either one of these patterns:

* If the project is created based on an opportunity or account trigger, the name of the project is: < * Salesforce object name>: <Project template name> (via Salesforce).*
* If the project is created based on an opportunity trigger that also includes the addition of a new Product, the name of the project is: < * Salesforce object name>: <Salesforce product name> (via Salesforce).*

## View *Workfront* projects

If your *Workfront administrator* added the *Workfront* section to your Opportunity or Account page layout, you can see the projects automatically created in the Projects tab of this section.  
For more information about adding the *Workfront* section to the page layout of an Opportunity or Account, see [Configure the Adobe Workfront section for Salesforce users](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

You must have a *Workfront* account and be logged in to *Workfront* to view the Projects tab.

To view projects created from an Opportunity or Account:&nbsp;

<ol> 
 <li value="1">Go to an Opportunity or Account.</li> 
 <li value="2"> <p>Go to the <span class="bold"><em>Workfront</em></span> section.</p> <note type="note">
   Depending on how your 
   <em>Workfront administrator</em> configured this section, it might have a different name.
  </note> </li> 
 <li value="3"> <p>Select the <span class="bold">Projects</span> tab.</p> <p>All projects created by defined triggers are listed in this tab. Any user in Salesforce who also has a <em>Workfront</em> account and who might have permissions to see these projects in <em>Workfront</em> can also see them in Salesforce for the Opportunity or the Account that generated them.</p> <p> <img src="assets/salesforce-projects-tab-with-projects-listed-350x150.png" alt="salesforce_projects_tab_with_projects_listed.png" style="width: 350;height: 150;"> </p> <p>You can view the following information about the projects created by the integration:</p> 
  <ul> 
   <li>Project Name&nbsp;</li> 
   <li>Reference Number</li> 
   <li>Entry Date</li> 
   <li>Name of the Owner</li> 
   <li>Status</li> 
   <li>Condition</li> 
   <li>Planned Completion Date</li> 
   <li>Percent Complete<span class="bold"><br></span>When this information is updated in <em>Workfront</em>, you can see the fields updated in this list.&nbsp;</li> 
  </ul> </li> 
 <li value="4">(Optional) Click the name of a project to open it in <em>Workfront</em>.&nbsp;</li> 
 <li value="5"> <p>(Optional) Click <span class="bold">Go to Salesforce</span> to access the Opportunity or Account where the project originated.</p> <note type="note">
   The Go to Salesforce link is visible to all 
   <em>Workfront</em> users who can view the project. You must have a Salesforce account to be able to go to the Salesforce Opportunity or Account from where the project was generated.&nbsp;&nbsp;
  </note> </li> 
</ol>

