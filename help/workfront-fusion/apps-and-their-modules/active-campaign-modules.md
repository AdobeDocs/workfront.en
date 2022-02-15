---
filename: active-campaign-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
---




# ActiveCampaign modules {#activecampaign-modules}

In a `Workfront Fusion 2.0` scenario, you can connect your `ActiveCampaign` account to multiple third-party applications and services. You can create, update, list, and delete automations, campaigns, calendar feeds, contacts, deals, messages, notes, organizations, tags, and tasks in your ActiveCampaign account.


If you need instructions on creating a scenario, see [Create a scenario](create-a-scenario.md). For information about modules, see [Modules](_modules.md).


## Connect Active Campaign to `Workfront Fusion 2.0` {#connect-active-campaign-to-workfront-fusion}




1. Log in to your ActiveCampaign account.
1. From the left menu, click **Settings** > **Developer**.

1. Copy the API **Key** to the clipboard.
1.  Go to `Workfront Fusion 2.0`, add an ActiveCampaign module to a scenario, and open the **Create a Connection** box, 


   If you need instructions, see [About connecting Workfront Fusion 2.0 to an app or service](about-connecting-wf-fusion-to-app-or-service.md).

1. In the API Key field, enter the API Key copied in step 3.
1.  In the Account name field, enter the account name in your ActiveCampaign URL.


   For example, if your URL is

   ```
   live1.activehosted.com
   ```

   then the account name is 

   ```
   live1
   ```

   .

1. Click **Continue**.




## ActiveCampaign Contact modules {#activecampaign-contact-modules}




* [Create a Contact](#create) 
* [Create/Update a Contact](#create/u) 
* [Delete a Contact](#delete) 
* [Get a Contact](#get) 
* [Create/Update a Contact's Custom Field Value](#create/u2) 
* [Update Contact's List Status](#update) 
* [Add a Tag to a Contact](#add) 
* [Remove a Tag from a Contact](#remove) 
* [List Contacts](#list) 
* [Get Info About Logged-in User](#get2) 
* [Watch Contacts](#watch) 




### Create a Contact {#create-a-contact}

This action module `creates a new contact``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


You specify the person's contact information.


The module returns the ID of the `<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  <span class="Snippet VariablesFusionAction">new</span> </MadCap:conditionalText>` `contact` and any associated fields, along with any custom fields and values that the connection accesses. You can map `this information` in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray"><b>Connection </b> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray"><b>Email </b> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Enter the email address of the contact.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray"><b>First Name</b> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p> Enter the first name of the contact.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray"><b>Last Name</b> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p> Enter the last name of the contact.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray"><b>Phone </b> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Enter the phone number of the contact.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Create/Update a Contact {#create-update-a-contact}

This action module `creates a new contact or updates an existing contact``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


You specify the contact information.


The module returns the ID of the `<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  <span class="Snippet VariablesFusionAction">new or updated</span> </MadCap:conditionalText>` `contact` and any associated fields, along with any custom fields and values that the connection accesses. You can map `this information` in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Connection </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Email </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Enter the email address of the contact.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>First Name</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> Enter the first name of the contact.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Last Name</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Enter the last name of the contact.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"><b>Phone </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>Enter the phone number of the contact.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Delete a Contact {#delete-a-contact}

This action module `deletes an existing contact``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


You specify the ID of the `contact`.


The module returns the ID of the `<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  <span class="Snippet VariablesFusionAction">deleted</span> </MadCap:conditionalText>` `contact` and any associated fields, along with any custom fields and values that the connection accesses. You can map `this information` in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Connection </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"><b>ID </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>Enter the unique <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> ID of the <span class="Snippet VariablesFusion-Record">contact</span> that you want the module to delete.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Get a Contact {#get-a-contact}

This action module `retrieves a contact``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


You specify the ID of the `contact`.


The module returns the ID of the `contact` and any associated fields, along with any custom fields and values that the connection accesses. You can map `this information` in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Connection </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"><b>ID </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>Select the type of <span class="Snippet VariablesFusion-Apps">[Fusion app]</span> record from which you want the module to retrieve details.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Create/Update a Contact's Custom Field Value {#create-update-a-contacts-custom-field-value}

This action module `creates or updates a custom field value for the given contact``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Connection </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Contact ID</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Select the Contact ID whose Custom Field value you want to update.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Field ID</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p><![CDATA[	]]>Enter the unique <span class="Snippet VariablesFusion-Apps">[Fusion app]</span> ID of the <span class="Snippet VariablesFusion-Record">record</span> that you want the module to update.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Field Value</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Enter the new field value to update.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"><b>Contact's field ID</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p> Enter the ID of the contact field to edit.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Update Contact's List Status {#update-contacts-list-status}

This action module `updates the list status for a contact``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


You specify the contact ID, list ID, and status.


The module returns the ID of the `<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  <span class="Snippet VariablesFusionAction">updated</span> </MadCap:conditionalText>` `status` and any associated fields, along with any custom fields and values that the connection accesses. You can map `this information` in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Connection </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Contact ID</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Select the Contact ID whose list status you want to update.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>List ID</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> Select the List ID of the contacts you want to update.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"> <p><b>Status</b> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>Select the status to update:</p> 
    <ul> 
     <li value="1">Active</li> 
     <li value="2">Unsubscribed</li> 
     <li value="3">Bounced</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>



### Add a Tag to a Contact {#add-a-tag-to-a-contact}

This action module `adds a tag to a contact``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


You specify the IDs of the contact and of the tag.


The module returns the ID of the `<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  <span class="Snippet VariablesFusionAction">new</span> </MadCap:conditionalText>` `tag and contact` and any associated fields, along with any custom fields and values that the connection accesses. You can map `this information` in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Connection </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Contact ID</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Enter the Contact ID to which you want to add the tag.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"><b>Tag ID</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p> Enter the Tag ID you want to add to the contact.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Remove a Tag from a Contact {#remove-a-tag-from-a-contact}

This action module `removes a tag from a contact``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


You specify the ID of the `contact`.


The module returns the ID of the `<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  <span class="Snippet VariablesFusionAction">new</span> </MadCap:conditionalText>` `contact tag` and any associated fields, along with any custom fields and values that the connection accesses. You can map `this information` in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Connection </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"><b>Contact's Tag ID</b><![CDATA[	]]></td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>Enter the Tag ID to remove from the contact.</p> </td> 
  </tr> 
 </tbody> 
</table>



### List Contacts {#list-contacts}

This action module `retrieves a list of contacts``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Connection </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Limit </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The maximum number of contacts should return during one scenario execution cycle.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p><b>Order by</b> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Select the order in which you want to list the contacts:</p> 
    <ul> 
     <li value="1">Creation date</li> 
     <li value="2">Email</li> 
     <li value="3">Name</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>ASC/DESC</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Select the order to list the contacts:</p> 
    <ul> 
     <li value="1">ASC - Ascending order</li> 
     <li value="2">DESC - Descending order</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Email </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Enter the email address of the contacts you want to list.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Email-like pattern</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Enter the email pattern to list the contacts that contain the given value in the email address.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Search pattern</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> Enter the search pattern to list contacts that match the given value in the contact names, organization, phone or email.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Organization ID</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Select the Organization ID whose contacts you want to list.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>List ID</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> Select the List ID of the contacts you want to list.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Segment ID</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Select the Segment ID whose contacts you want to list.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Status</b><![CDATA[	]]></td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Select the status of the contacts you want to list:</p> 
    <ul> 
     <li value="1">Any</li> 
     <li value="2">Unconfirmed</li> 
     <li value="3">Active</li> 
     <li value="4">Unsubscribed</li> 
     <li value="5">Bounced</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Tag ID</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Select the Tag ID for the contact.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Form ID</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> Select the Form ID for the contact.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Since DateTime</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Select the date from which you want to list the contacts.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"><b>Until DateTime</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p> Select the date until which you want to list the contacts.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Get Info About Logged-in User {#get-info-about-logged-in-user}

This action module `gets information about the logged-in users``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"><b>Connection </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Watch Contacts {#watch-contacts}

This trigger module executes a scenario when `a new contact is created``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`. The module `returns all standard fields associated with the record or records, along with any custom fields and values that the connection accesses`.You can map `this information` in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Connection </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Limit </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The maximum number of contacts should return during one scenario execution cycle.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Email </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Enter the email address of the contacts you want to watch.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Email-like Pattern</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Enter the email pattern to list the contacts that contain the given value in the email address.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Search Pattern</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> Enter the search pattern to list contacts that match the given value in the contact names, organization, phone or email.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Organization ID</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Select the Organization ID whose contacts you want to watch.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>List ID</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> Select the List ID of the contacts you want to watch.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Segment ID</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Select the Segment ID whose contacts you want to watch.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Status </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Select the status of the contacts you want to watch:</p> 
    <ul> 
     <li value="1">Any</li> 
     <li value="2">Unconfirmed</li> 
     <li value="3">Active</li> 
     <li value="4">Unsubscribed</li> 
     <li value="5">Bounced</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Tag ID</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Select the Tag ID whose contacts you want to watch.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Form ID</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> Select the Form ID for the contact you want to watch.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Since DateTime</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Select the date from which you want to watch the contacts.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"><b>Until DateTime</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p> Select the date until which you want to watch the contacts.</p> </td> 
  </tr> 
 </tbody> 
</table>



## ActiveCampaign Deal modules {#activecampaign-deal-modules}




* [Create a Deal](#create3) 
* [Update a Deal](#update3) 
* [Get a Deal](#get4) 
* [Delete a Deal](#delete2) 
* [Move Details to Another Deal Stage](#move) 
* [List Deals](#list3) 
* [Watch Deals](#watch3) 




### Create a Deal {#create-a-deal}

This action module `creates a new deal``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


You specify information about the deal.


The module returns the ID of the `deal` and any associated fields, along with any custom fields and values that the connection accesses. You can map `this information` in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Connection </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: normal;"><b>Title </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Enter the name of the deal.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Description </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Enter the details of the deal.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Contact ID</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Select the Contact ID to assign the deal.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Pipeline ID </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Select the Pipeline ID for the deal.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Stage </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Enter the stage name of the deal.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Owner ID</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> Select the Owner ID to assign as the deal owner.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Value </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Enter the deal value in cents.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Currency </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Select the currency applicable for the deal.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Percent </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Enter the deal's percentage.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Status </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Select the status of the deal:</p> 
    <ul> 
     <li value="1">Open</li> 
     <li value="2">Lost</li> 
     <li value="3">Won</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"> <p><b>Custom Fields</b> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>Add the custom fields.</p> 
    <ul> 
     <li value="1"> <p>Custom Field ID</p> <p>Select the Custom Field ID.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>



### Update a Deal {#update-a-deal}

This action module `updates an existing deal``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


You specify the new information about the deal.


The module returns the ID of the `<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  <span class="Snippet VariablesFusionAction">updated</span> </MadCap:conditionalText>` `deal` and any associated fields, along with any custom fields and values that the connection accesses. You can map `this information` in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 201px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Connection </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Deal ID</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Select the Deal ID you want to update.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Title </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Enter the name for the deal.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Description</b><![CDATA[	]]></td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Enter the details for the deal.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p><b>Contact ID</b> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Select the Contact ID to assign the deal.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Pipeline ID</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Select the Pipeline ID for the deal.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Stage </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Enter the stage name of the deal.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Owner ID</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Select the Owner ID to assign as the deal owner.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Value </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Enter the deal value in cents.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Currency </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Select the currency applicable for the deal.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Percent </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Enter the deal's percentage.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"><b>Status </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>Select the status of the deal:</p> 
    <ul> 
     <li value="1">Open</li> 
     <li value="2">Lost</li> 
     <li value="3">Won</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>



### Get a Deal {#get-a-deal}

This action module `returns a deal``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


You specify the ID of the `deal`.


The module returns the ID of the `deal` and any associated fields, along with any custom fields and values that the connection accesses. You can map `this information` in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Connection </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"><b>ID </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>Enter the Deal ID whose details you want to retrieve.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Delete a Deal {#delete-a-deal}

This action module `deletes an existing deal``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


You specify the ID of the `deal`.


The module returns the ID of the `<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  <span class="Snippet VariablesFusionAction">deleted</span> </MadCap:conditionalText>` `deal` and any associated fields, along with any custom fields and values that the connection accesses. You can map `this information` in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Connection </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"><b>ID </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>Select the Deal ID you want to delete.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Move Details to Another Deal Stage {#move-details-to-another-deal-stage}

This action module `moves all deals in one stage to another stage``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


You specify the IDs of the stage and of the target stage.


The module returns the ID of the `<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  <span class="Snippet VariablesFusionAction">moved</span> </MadCap:conditionalText>` `stage` and any associated fields, along with any custom fields and values that the connection accesses. You can map `this information` in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Connection </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Stage ID</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Select the Stage ID whose details you want to move to another stage.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"><b>Target stage ID</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p> Select the Stage ID to which you want to move the details.</p> </td> 
  </tr> 
 </tbody> 
</table>



### List Deals {#list-deals}

This action module `retrieves a list of deals``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Connection </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: normal;"><b>Limit </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The maximum number of deals should return during one scenario execution cycle.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Group </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Enter the group name of the deal you want to list.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Stage </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Enter the stage name of the deals you want to list.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Owner </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Enter the owner name of the deals you want to list.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Status </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Enter the status of the deals you want to list.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Due date</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> Enter the due date of the deal that you want to list.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: normal;"><b>Tag </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Enter the tag names to filter the deals.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Task Type</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> Select the task type of the deal that you want to list.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Created Before</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Enter the date from which the deals that you want to list were created.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Created After</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> Enter the date from which the deals that you want to list were created.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Updated Before</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Enter the date before which the deals that you want to list were updated.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Updated After</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> Enter the date from which the deals that you want to list were updated.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"><b>Organization </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>Select the organization whose deals you want to list.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Watch Deals {#watch-deals}

This trigger module executes a scenario when `a deal is created``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`. The module `returns all standard fields associated with the record or records, along with any custom fields and values that the connection accesses`.You can map `this information` in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Connection </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Limit </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The maximum number of deals should return during one scenario execution cycle.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Title </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Enter the name to filter the deal you want to watch.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Group </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Enter the group name of the deals you want to watch.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: normal;"><b>Stage </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Enter the stage name of the deals you want to watch.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Owner </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Enter the owner name of the deals you want to watch</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Status </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Enter the status of the deals you want to watch.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Due Date</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Enter the due date of the deal that you want to watch.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Tag </b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Enter the tag names to filter the deals.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Task Type</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Select the task type of the deal that you want to watch.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Created Before</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> Enter the date from which the deals that you want to watch were created.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Created After</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Enter the date from which the deals that you want to watch were created.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Updated Before</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> Enter the date before which the deals that you want to watch were updated.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><b>Updated After</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Enter the date from which the deals that you want to watch were updated.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"><b>Organization</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p> Select the organization whose deals you want to watch.</p> </td> 
  </tr> 
 </tbody> 
</table>



## ActiveCampaign Campaign modules {#activecampaign-campaign-modules}




* [Get a Campaign](#get5) 
* [Delete a Campaign](#delete3) 
* [List Campaigns](#list4) 




### Get a Campaign {#get-a-campaign}

This action module `retrieves a campaign``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


You specify the ID of the `campaign`.


The module returns the ID of the `campaign` and any associated fields, along with any custom fields and values that the connection accesses. You can map `this information` in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">ID </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>Enter the Campaign ID whose details you want to retrieve.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Delete a Campaign {#delete-a-campaign}

This action module `deletes an existing campaign``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


You specify the ID of the `campaign`.


The module returns the ID of the `<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  <span class="Snippet VariablesFusionAction">deleted</span> </MadCap:conditionalText>` `campaign` and any associated fields, along with any custom fields and values that the connection accesses. You can map `this information` in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">ID </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>Enter the unique <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> ID of the <span class="Snippet VariablesFusion-Record">campaign</span> that you want the module to </p> <p>delete.</p> </td> 
  </tr> 
 </tbody> 
</table>



### List Campaigns {#list-campaigns}

This action module `retrieves a list of campaigns``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


You specify the highest number of records you want the module to list during each scenario execution cycle.


The module returns the ID of the `list` and any associated fields, along with any custom fields and values that the connection accesses. You can map `this information` in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">Limit</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>Type the highest number of <span class="Snippet VariablesFusion-Record">record</span>s you want the module to <span class="Snippet VariablesFusionAction">list</span> during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>



## ActiveCampaign Task modules {#activecampaign-task-modules}




* [Create/Update a Task](#create/u4) 
* [Delete a Task](#delete4) 
* [Watch Tasks](#watch4) 




### Create/Update a Task {#create-update-a-task}

This action module `creates a new task or updates an existing task``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


You specify information about the task.


The module returns the ID of the `<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  <span class="Snippet VariablesFusionAction">new or updated</span> </MadCap:conditionalText>` `task` and any associated fields, along with any custom fields and values that the connection accesses. You can map `this information` in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">Owner type</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Select the task owner type of the task you want to create:</p> 
    <ul> 
     <li value="1">Deal</li> 
     <li value="2">Contact</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Due Date </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Enter the date by which the task must be completed.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">End Date</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Enter the date on which the task expires.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Task Type</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> Select the task type:</p> 
    <ul> 
     <li value="1">Calls</li> 
     <li value="2">Email</li> 
     <li value="3">Lunch</li> 
     <li value="4">Meeting</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">Title </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Enter the name of the task.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Status </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Enter the status of the task.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">Note </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Enter the details of the task.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray" style="font-weight: bold;">ID </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>Enter the Task ID to update.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Delete a Task {#delete-a-task}

This action module `deletes an existing task``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


You specify the ID of the `task`.


The module returns the ID of the `<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  <span class="Snippet VariablesFusionAction">deleted</span> </MadCap:conditionalText>` `task` and any associated fields, along with any custom fields and values that the connection accesses. You can map `this information` in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">ID </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>Select the Task ID you want to delete.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Watch Tasks {#watch-tasks}

This trigger module executes a scenario when `a new task is assigned to a deal``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`. The module `returns all standard fields associated with the record or records, along with any custom fields and values that the connection accesses`.You can map `this information` in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Connection </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Limit </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>The maximum number of tasks should return during one scenario execution cycle.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Title </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Enter the name to filter the tasks.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Deal ID</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p> Select the Deal ID whose tasks you want to watch.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Status </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Select the status of the task you want to watch.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Note </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Enter the note to filter the task you want to watch.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Due Date</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p> Enter the due date of the task you want to watch.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray">Task Type</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p> Select the task type you want to watch:</p> 
    <ul> 
     <li value="1">Call</li> 
     <li value="2">Email</li> 
     <li value="3">Lunch</li> 
     <li value="4">Meeting</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>



## ActiveCampaign Note modules {#activecampaign-note-modules}




* [Create a Note](#create5) 
* [Create a Deal Note](#create6) 




### Create a Note {#create-a-note}

This action module `adds a note to an activity, a deal, a deal task, or to a subscriber``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


You specify the note and the object.


The module returns the ID of the `<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  <span class="Snippet VariablesFusionAction">new</span> </MadCap:conditionalText>` `note` and any associated fields, along with any custom fields and values that the connection accesses. You can map `this information` in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Connection</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Note</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Enter the note text</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Associated Object ID</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Enter the ID of the object whose note you are creating.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray">Associated Object Type</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">Select the object type.</td> 
  </tr> 
 </tbody> 
</table>



### Create a Deal Note {#create-a-deal-note}

This action module `creates a new note for a deal``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


You specify the note and the ID of the deal.


The module returns the ID of the `<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  <span class="Snippet VariablesFusionAction">new</span> </MadCap:conditionalText>` `note` and any associated fields, along with any custom fields and values that the connection accesses. You can map `this information` in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">ID </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Enter the Deal ID to which you want to create a deal note.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray" style="font-weight: bold;">Note </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>Enter the note to add to the deal.</p> </td> 
  </tr> 
 </tbody> 
</table>



## ActiveCampaign Automation modules {#activecampaign-automation-modules}




* [List Automations](#list6) 
* [List Organizations](#list7) 
* [Add a Contact to an Automation](#add3) 
* [Get an Automation a Contact Is In](#get6) 
* [Remove a Contact from an Automation](#remove2) 
* [List All Automations a Contacts Is In](#list8) 




### List Automations {#list-automations}

This action module `retrieves a list of automations``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


You specify the highest number of records you want the module to list during each scenario execution cycle.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">Limit </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>Type the highest number of <span class="Snippet VariablesFusion-Record">record</span>s you want the module to <span class="Snippet VariablesFusionAction">[action]</span> during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>



### List Organizations {#list-organizations}

This action module `retrieves a list of organizations``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">Limit </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>The maximum number of organizations should return during one scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Add a Contact to an Automation {#add-a-contact-to-an-automation}

This action module `adds a contact to an automation``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


You specify the IDs of the contact and of the automation.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p style="font-weight: bold;">Contact ID</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Select the Contact ID you want to add to an automation.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> <p style="font-weight: bold;">Automation ID</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>Select the Automation ID to which you want to add the contact.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Get an Automation a Contact Is In {#get-an-automation-a-contact-is-in}

This action module `retrieves an automation that contains a contact``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


You specify the ID of the `contact`.


The module returns the ID of the `automation` and any associated fields, along with any custom fields and values that the connection accesses. You can map `this information` in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">ID </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>Enter the Contact ID whose details you want to retrieve.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Remove a Contact from an Automation {#remove-a-contact-from-an-automation}

This action module `removes a contact from an automation``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


You specify the ID of the `contact`.


The module returns the ID of the `<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  <span class="Snippet VariablesFusionAction">removed</span> </MadCap:conditionalText>` `contact` and any associated fields, along with any custom fields and values that the connection accesses. You can map `this information` in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">ID </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>Select the Contact ID you want to remove from an automation.</p> </td> 
  </tr> 
 </tbody> 
</table>



### List All Automations a Contacts Is In {#list-all-automations-a-contacts-is-in}

This action module `retrieves a list of automations that contain a contact``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


You specify the maximum number of automations you want to list.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">Limit </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>The maximum number of automations you want listed during 1 execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>



## ActiveCampaign Message modules {#activecampaign-message-modules}



### Create a Message {#create-a-message}

This action module `creates a message``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


You specify the information for the message.


The module returns the ID of the `<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  <span class="Snippet VariablesFusionAction">new</span> </MadCap:conditionalText>` `message` and any associated fields, along with any custom fields and values that the connection accesses. You can map `this information` in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">From Name</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Enter the name from whom the message will be sent.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">From Email </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Enter the email address from which the message will be sent.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">Reply Email </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Enter the email address to send the reply</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Subject</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> Enter the message subject.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">Preheader Text </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>Enter the preheader text for the message.</p> </td> 
  </tr> 
 </tbody> 
</table>



## ActiveCampaign Calendar Feed modules {#activecampaign-calendar-feed-modules}




* [Create/Update a Calendar Feed](#create/u5) 
* [Delete a Calendar Feed](#delete5) 
* [Watch Calendar Feeds](#watch6) 




### Create/Update a Calendar Feed {#create-update-a-calendar-feed}

This action module `creates or updates a calendar feed``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


You specify information about the feed.


The module returns the ID of the `<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  <span class="Snippet VariablesFusionAction">new or updated</span> </MadCap:conditionalText>` `feed` and any associated fields, along with any custom fields and values that the connection accesses. You can map `this information` in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">Title </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Enter the name of the calendar feed.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Type </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Enter the calendar feed type:</p> 
    <ul> 
     <li value="1">All</li> 
     <li value="2">Deals</li> 
     <li value="3">Contacts</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">Notification flag</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> 
    <ul> 
     <li value="1"> Select Yes if this calendar feed has notifications:</li> 
     <li value="2">Yes</li> 
     <li value="3">No</li> 
     <li value="4">Not defined</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray" style="font-weight: bold;">ID </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>Select the Calendar Feed ID you want to update.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Delete a Calendar Feed {#delete-a-calendar-feed}

This action module `deletes a calendar feed``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


You specify the ID of the `record`.


The module returns the ID of the `<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  <span class="Snippet VariablesFusionAction">deleted</span> </MadCap:conditionalText>` `calendar feed` and any associated fields, along with any custom fields and values that the connection accesses. You can map `this information` in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">ID </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>Select the Calendar Feed ID you want to delete.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Watch Calendar Feeds {#watch-calendar-feeds}

This trigger module executes a scenario when `a new calendar feed is created or updated``<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span></MadCap:conditionalText>`.


The module `returns all standard fields associated with the record or records, along with any custom fields and values that the connection accesses`.You can map `this information` in subsequent modules in the scenario.


You specify the maximum number of calendar feeds that you want listed.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">Limit </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>The maximum number of calendar feeds should return during one scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Troubleshooting {#troubleshooting}

The trigger for watching all automations associated with a contact returns dates without time zones. It is a bug in the API, v.2.


### How to connect to an ActiveCampaign List with Webhook {#how-to-connect-to-an-activecampaign-list-with-webhook}




1. Add a Watch events module to your scenario.
1.  Set up the webhook.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col style="width: 199px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your <span class="Snippet VariablesFusion-Apps">ActiveCampaign</span> account to <span class="WFVariablesProdNameWFF">Workfront Fusion 2.0</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Active Campaign to Workfront Fusion 2.0</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">Custom Webhook Name</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Enter the name for your webhook. E.g. Contacts Webhook.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Events </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Select events that will trigger the webhook.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">Sources </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>Select who initates the webhook, whether it is contact, admin, API, or system processes.</p> </td> 
  </tr> 
 </tbody> 
</table>


1. Save your setting by clicking the **Save** button, then close and save the Watch events webhook module by clicking **OK**.

1. Log in to your ActiveCampaign account.
1.  In the **Settings** dropdown menu, click **Developer**, then click **Manage Webhooks**.
1.  In the Webhook settings fields, click **Edit** to open the webhook settings in the ActiveCampaign.
1.  In the Webhook settings section, in the **List** dropdown menu, select the list that you want to work with the `Workfront Fusion 2.0` webhook.
1. Run your scenario in `Workfront Fusion 2.0` and then **send sample Data** so that you can confirm if the webhook catches the correct data.

1.   **Update** to save your work.


