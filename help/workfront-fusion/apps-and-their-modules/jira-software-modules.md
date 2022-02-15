


# Jira Software modules {#jira-software-modules}

In a *`Adobe Workfront Fusion`* scenario, you can connect your *`Jira Software`* account to multiple third-party applications and services.


If you need instructions on creating a scenario, see [Create a scenario](create-a-scenario.md). 


For information about modules, see [Modules in Adobe Workfront Fusion](_modules.md).


## Access requirements {#access-requirements}

You must have the following access to use the functionality in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p><span class="mc-variable WFVariables.WFPlan-Pro variable varname">Pro</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWFF variable varname">Adobe Workfront Fusion</span> license**</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFFusionIntegration variable varname">Workfront Fusion for Work Automation and Integration</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Product</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Your organization must purchase <span class="mc-variable WFVariables.FullProdNameWFF variable varname">Adobe Workfront Fusion</span> as well as <span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Prerequisites {#prerequisites}

To use Jira modules you must have a Jira account.


## Connect Jira Software to *`Workfront Fusion`* {#connect-jira-software-to-workfront-fusion}

Your connection method is based on whether you are using Jira Cloud or Jira Server. 



* [Connect Jira Cloud to Workfront Fusion](#connect) 
* [Connect Jira Server to Workfront Fusion](#connect2) 




### Connect Jira Cloud to *`Workfront Fusion`* {#connect-jira-cloud-to-workfront-fusion}

Connect Jira Cloud to *`Workfront Fusion`*


To connect Jira Software to *`Workfront Fusion`*, you must create an API token and insert it together with your Service URL and Username to the Create a connection field in *`Workfront Fusion`*.


#### Create an API&nbsp;token in Jira {#create-an-api-token-in-jira}




1. Go to [https://id.atlassian.com/manage/api-tokens](https://id.atlassian.com/manage/api-tokens) and log in.
1. Click `Create API token`.
1. Type a name for the token, such as *Workfront Fusion*.
1.  Copy the token using the `Copy to clipboard` button.


   >[!IMPORTANT] {type="important"}
   >
   >You can't view the token again after closing this dialog.



1. Store the generated token in a safe place.
1. Continue with [Configure the Jira API token in Workfront Fusion](#configur2).




#### Configure the Jira API token in *`Workfront Fusion`* {#configure-the-jira-api-token-in-workfront-fusion}




1. In *`Workfront Fusion`*, add a Jira module to a scenario to open the `Create a connection` box.

1. Specify the following information:
    
    
    * `Service URL:`
    * `Username:`
    * `API token:`&nbsp;This is the API token you created in the [Create an API token in Jira](#create3) section of this article.
    
    
    
1. Click Continue to create the connection and return to the module.





### Connect Jira Server to *`Workfront Fusion`* {#connect-jira-server-to-workfront-fusion}

To authorize a connection between *`Workfront Fusion`* and Jira Server, you need your Consumer Key, Private Key, And Service URL. You might need to contact your Jira administrator for this information.



*  [Generate Public and Private keys for your Jira connection](#generate) 
*  [Configure the client app as a consumer in Jira](#configur) 
*  [Create a connection to Jira Server or Jira Data Center in Workfront Fusion](#create2) 




#### Generate Public and Private keys for your Jira connection {#generate-public-and-private-keys-for-your-jira-connection}

To acquire a private key for your *`Workfront Fusion`* Jira connection, you need to generate public and private keys. 



1.  In your terminal, run the following 

   ```
   openssl
   ```

   commands.

    
    
    * `<pre>openssl genrsa -out jira_privatekey.pem 1024</pre>` This command generates a 1024 bit private key.
    
    * `<pre>openssl req -newkey rsa:1024 -x509 -key jira_privatekey.pem -out jira_publickey.cer -days 365</pre>` This command creates an X509 certificate.
    
    * `<pre>openssl pkcs8 -topk8 -nocrypt -in jira_privatekey.pem -out jira_privatekey.pcks8</pre>` This command extracts the private key (PKCS8 format) to the     
    
      ```    
      jira_privatekey.pcks8
      ```    
    
      file.
    
    * `<pre>openssl x509 -pubkey -noout -in jira_publickey.cer  > jira_publickey.pem</pre>` This command extracts the public key from the certificate to the    
    
      ```    
      jira_publickey.pem
      ```    
    
      file.
    
    
      >[!NOTE]
      >
      >If you are using Windows, you might need to save the public key to the       >
      >
      >```      >
      >jira_publickey.pem
      >```      >
      >
      >file manually:
      >
      >    
      >    
      >    1.  In your terminal, run the following command:
      >    
      >    
      >       openssl x509 -pubkey -noout -in jira_publickey.cer 
      >    
      >    1. Copy the terminal output (including       >    
      >    
      >       ```      >    
      >       -------BEGIN PUBLIC KEY--------
      >       ```      >    
      >    
      >       and       >    
      >    
      >       ```      >    
      >       -------END PUBLIC KEY--------
      >       ```      >    
      >    
      >    
      >    1. Paste the terminal output into a file named       >    
      >    
      >       ```      >    
      >       jira_publickey.pem
      >       ```      >    
      >    
      >       .
      >    
      >    

    
    
    
    
    

1.  Continue to [Configure the client app as a consumer in Jira](#configur)




#### Configure the client app as a consumer in Jira {#configure-the-client-app-as-a-consumer-in-jira}




1.  Log into your Jira instance.
1.  In the left navigation panel, click `Jira Settings` ![](assets/jira-settings-icon.png) > `Applications`> `Application links`.
1.  In the `Enter the URL of the application you want to link` field, enter 

   ```
   https://app.workfrontfusion.com/oauth/cb/workfront-jiraserver-oauth1
   ```


1.  Click `Create new link`. Ignore the "No response was received from the URL you entered" error message.
1.  In the `Link applications` window, enter values into the `Consumer key` and `Shared secret` fields. You can choose the values for these fields. 
1.  Copy the values of the `Consumer key` and `Shared secret` fields to a secure location. You will require these values later in the configuration process.
1.  Fill in the URL fields as follows:


1.  Select the `Create incoming link` checkbox.
1.  Click `Continue`.
1.   the `Link applications` window, fill in the following fields:

<table style="mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" data-mc-conditions=""> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" data-mc-conditions=""> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <p>Consumer Key</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> Paste in the consumer key that you copied to a secure location.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Consumer name</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Enter a name of your choice. This name is for your own reference.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Public key</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Paste in the public key from your <code>jira_publickey.pem</code> file.</td> 
  </tr> 
 </tbody> 
</table>


1.  Click `Continue`
1.  Continue to [Create a connection to Jira Server or Jira Data Center in Workfront Fusion](#create2)




#### Create a connection to Jira Server or Jira Data Center in *`Workfront Fusion`* {#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion}



>[!NOTE]
>
>Use the Jira Server app to connect to Jira Server or Jira Data Center.





1. In any Jira Server module in *`Workfront Fusion`*, click `Add` next to the connection field.

1.  In the Create a connection panel, fill in the following fields:

<table style="mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <p>Connection name</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Enter a name for the connection</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Consumer Key</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Paste in the consumer key that you copied to a secure location in <a href="#configur" class="MCXref xref">Configure the client app as a consumer in Jira</a></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Private Key</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Paste in the private key from the <code>jira_privatekey.pcks8</code> file you created in <a href="#generate" class="MCXref xref">Generate Public and Private keys for your Jira connection</a>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Service URL</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">Enter your Jira instance URL. </td> 
  </tr> 
 </tbody> 
</table>


1. Click `Continue` to create the connection and go back to the module.




## Jira Software modules and their fields {#jira-software-modules-and-their-fields}

When you configure *`Jira Software`* modules, *`Workfront Fusion`* displays the fields listed below. Along with these, additional *`Jira Software`* fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.


If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another](map-information-between-modules.md).


![](assets/map-toggle-350x74.png)





* [Triggers](#triggers) 
* [Actions](#actions) 
* [Searches](#searches) 




### Triggers {#triggers}



#### Watch for records {#watch-for-records}

This trigger module starts a scenario when a record is added, updated, or deleted.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Webhook</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Select the webhook that you want to use to watch for records. </p> <p>To add a new webhook:</p> 
    <ol> 
     <li value="1">Click <span class="bold">Add</span></li> 
     <li value="2">Enter a name for the webhook.</li> 
     <li value="3"> <p>Select the connection you want to use for your webhook. </p> <p>For instructions about connecting your <span class="mc-variable Snippet_Variables.Fusion-Apps variable varname">Jira Software</span> account to <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Jira Cloud to Workfront Fusion</a> in this article.</p> </li> 
     <li value="4"> <p>Select the record type that you want the software to watch for:</p> 
      <ul> 
       <li>Comment </li> 
       <li>Issue</li> 
       <li>Project </li> 
       <li>Sprint</li> 
      </ul> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>



### Actions {#actions}




* [Add issue to sprint](#add) 
* [Custom API Call](#custom) 
* [Create a Record](#create) 
* [Delete a record](#delete) 
* [Download an attachment](#download) 
* [Read a record](#read) 
* [Update a record](#update) 




#### Add issue to sprint {#add-issue-to-sprint}

This action module *`adds one or more issues to a sprint`*`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="mc-variable Snippet_Variables.Fusion-Apps variable varname">Jira Software</span></MadCap:conditionalText>`.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="mc-variable Snippet_Variables.Fusion-Apps variable varname">Jira Software</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Connection</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>For instructions about connecting your <span class="mc-variable Snippet_Variables.Fusion-Apps variable varname">Jira Software</span> account to <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Jira Cloud to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Sprint ID</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Enter or map the Sprint ID of the sprint that you want to add an issue to.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Issue ID or Keys</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Add an Issue ID or Key for each issue you want to add to the sprint.</td> 
  </tr> 
 </tbody> 
</table>



#### Create a Record {#create-a-record}

This action module creates a new record in Jira.


The module returns any standard fields associated with the record`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  or records</MadCap:conditionalText>`, along with any custom fields and values that the connection accesses. You can map *`this information`* in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="mc-variable Snippet_Variables.Fusion-Apps variable varname">Jira Software</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Connection</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>For instructions about connecting your <span class="mc-variable Snippet_Variables.Fusion-Apps variable varname">Jira Software</span> account to <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Jira Cloud to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Record Type</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Select the type of record you want the module to create. When you select a record type, other fields specific to that record type appear in the module.</p> 
    <ul> 
     <li>Attachment</li> 
     <li>Comment</li> 
     <li>Issue</li> 
     <li>Project</li> 
     <li>Sprint </li> 
     <li>Worklog</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>



#### Custom API Call {#custom-api-call}

This action module lets you make a custom authenticated call to the *`Jira Software`* API`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  without having to think through authentication</MadCap:conditionalText>`. This way, you can create a data flow automation that can't be accomplished by the other *`Jira Software`* modules. 


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="mc-variable Snippet_Variables.Fusion-Apps variable varname">Jira Software</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" style="width: 320px;"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Connection</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>For instructions about connecting your <span class="mc-variable Snippet_Variables.Fusion-Apps variable varname">Jira Software</span> account to <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Jira Cloud to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">URL</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Enter a path relative to<code>&lt;Instance URL&gt;/rest/api/2/ </code></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Method</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Headers</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Add the headers of the request in the form of a standard JSON object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p><span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span> adds the authorization headers for you.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Query String</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Add the query for the API call in the form of a standard JSON object.</p> <p>For example: <code>{“name”:“something-urgent”}</code></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Body</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>



#### Delete a record {#delete-a-record}

This action module *`deletes a particular record`*`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="mc-variable Snippet_Variables.Fusion-Apps variable varname">Jira Software</span></MadCap:conditionalText>`.


You specify the`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  type and</MadCap:conditionalText>` ID of the *`record`*.


The module returns the ID of the `<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  <span class="mc-variable Snippet_Variables.FusionAction variable varname">deleted</span></MadCap:conditionalText>` *`record`* and any associated fields, along with any custom fields and values that the connection accesses. You can map *`this information`* in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="mc-variable Snippet_Variables.Fusion-Apps variable varname">Jira Software</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Connection</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>For instructions about connecting your <span class="mc-variable Snippet_Variables.Fusion-Apps variable varname">Jira Software</span> account to <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Jira Cloud to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Record Type</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Select the type of record you want the module to delete. </p> 
    <ul> 
     <li>Attachment</li> 
     <li>Comment</li> 
     <li>Issue</li> 
     <li>Project</li> 
     <li>Sprint </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">ID or Key</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Enter or map the ID or Key of the record you want to delete.</td> 
  </tr> 
 </tbody> 
</table>



#### Download an attachment {#download-an-attachment}

This action module *`downloads a particular attachment`*`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="mc-variable Snippet_Variables.Fusion-Apps variable varname">Jira Software</span></MadCap:conditionalText>`.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="mc-variable Snippet_Variables.Fusion-Apps variable varname">Jira Software</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Connection</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>For instructions about connecting your <span class="mc-variable Snippet_Variables.Fusion-Apps variable varname">Jira Software</span> account to <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Jira Cloud to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">ID</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">Enter or map the ID of the attachment you want to download.</td> 
  </tr> 
 </tbody> 
</table>



#### Read a record {#read-a-record}

This action module reads *`data from a single record`* in *`Jira Software`*.


You specify the`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  type and</MadCap:conditionalText>` ID of the *`record`*.


The module returns any standard fields associated with the record`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  or records</MadCap:conditionalText>`, along with any custom fields and values that the connection accesses. You can map *`this information`* in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="mc-variable Snippet_Variables.Fusion-Apps variable varname">Jira Software</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Connection</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>For instructions about connecting your <span class="mc-variable Snippet_Variables.Fusion-Apps variable varname">Jira Software</span> account to <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Jira Cloud to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Record Type</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Select the type of Jira record you want the module to read.</p> 
    <ul> 
     <li>Attachment</li> 
     <li>Issue</li> 
     <li>Project</li> 
     <li>Sprint </li> 
     <li>User</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Outputs</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Select the outputs that you want to receive. Output options are available based on the type of record selected in the "Record Type" field.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">ID</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Enter or map the unique <span class="mc-variable Snippet_Variables.Fusion-Apps variable varname">Jira Software</span> ID of the <span class="mc-variable Snippet_Variables.Fusion-Record variable varname">record</span> that you want the module to <span class="mc-variable Snippet_Variables.FusionAction variable varname">read</span>.</p> </td> 
  </tr> 
 </tbody> 
</table>



#### Update a record {#update-a-record}

This action module *`updates an existing record, such as an issue or project,`*`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <span class="mc-variable Snippet_Variables.Fusion-Apps variable varname">Jira Software</span></MadCap:conditionalText>`.


You specify the`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  type and</MadCap:conditionalText>` ID of the *`record`*.


The module returns the ID of the `<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  <span class="mc-variable Snippet_Variables.FusionAction variable varname">updated</span></MadCap:conditionalText>` *`record`* and any associated fields, along with any custom fields and values that the connection accesses. You can map *`this information`* in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="mc-variable Snippet_Variables.Fusion-Apps variable varname">Jira Software</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Connection</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>For instructions about connecting your <span class="mc-variable Snippet_Variables.Fusion-Apps variable varname">Jira Software</span> account to <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Jira Cloud to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Record Type</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Select the type of record you want the module to update. When you select a record type, other fields specific to that record type appear in the module.</p> 
    <ul> 
     <li>Comment</li> 
     <li>Issue</li> 
     <li>Project</li> 
     <li>Sprint </li> 
     <li>Transition issue</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">ID or Key</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Enter or map the ID or Key of the record you want to update.</td> 
  </tr> 
 </tbody> 
</table>



### Searches {#searches}




* [List records](#list) 
* [Search for records](#search) 




#### List records {#list-records}

This search module retrieves all items of a specific type that match your search query


`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> The module returns all standard fields associated with the record or records, along with any custom fields and values that the connection accesses.</MadCap:conditionalText>`You can map *`this information`* in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="mc-variable Snippet_Variables.Fusion-Apps variable varname">Jira Software</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Connection</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>For instructions about connecting your <span class="mc-variable Snippet_Variables.Fusion-Apps variable varname">Jira Software</span> account to <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Jira Cloud to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Record Type</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Select the type of record you want the module to list. When you select a record type, other fields specific to that record type appear in the module.</p> 
    <ul> 
     <li>Comment</li> 
     <li>Issue</li> 
     <li>Project</li> 
     <li>Sprint issue</li> 
     <li>Worklog</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader"> <p>Max Results</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Enter or map the maximum number of <span class="mc-variable Snippet_Variables.Fusion-Record variable varname">record</span>s you want the module to <span class="mc-variable Snippet_Variables.FusionAction variable varname">retrieve</span> during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>



#### Search for records {#search-for-records}

This search module looks for *`records in an object`* in *`Jira Software`* that match the search query you specify.


`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> The module  <span class="mc-variable Snippet_Variables.Fusion-ModuleReturns variable varname">returns all standard fields associated with the record or records, along with any custom fields and values that the connection accesses</span>.</MadCap:conditionalText>` You can map *`this information`* in subsequent modules in the scenario.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="mc-variable Snippet_Variables.Fusion-Apps variable varname">Jira Software</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Connection</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>For instructions about connecting your <span class="mc-variable Snippet_Variables.Fusion-Apps variable varname">Jira Software</span> account to <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Jira Cloud to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Record Type</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Select the type of record you want the module to search for. When you select a record type, other fields specific to that record type appear in the module.</p> 
    <ul> 
     <li>Issues</li> 
     <li> <p>Issues by JQL (Jira Query Lanuguage) </p> <p>For more information on JQL, see <a href="https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14#:~:text=JQL stands for Jira Query,project managers%2C and business users.">JQL</a> at the Atlassian help site. </p> </li> 
     <li>Project</li> 
     <li>Project by issue</li> 
     <li>User</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

