---
filename: aem-cloud-connector-setup
product-area: workfront-integrations;setup
navigation-topic: workfront-for-adobe-experience-manager
title: Set up the AEM cloud connector
description: This document explains how to include the Workfront Connector as a Maven dependency in AEM projects deployed to an AEM as a Cloud Service environment. The steps in this document refers to an AEM project called 'sample-site,' which acts as a stand-in for a client's site. The sample-site AEM project is based on Adobe's Maven archetype.
---

# Set up the AEM cloud connector

This document explains how to include the Workfront Connector as a Maven dependency in AEM projects deployed to an AEM as a Cloud Service environment. The steps in this document refers to an AEM project called 'sample-site,' which acts as a stand-in for a client's site. The sample-site AEM project is based on [Adobe's Maven archetype](https://github.com/adobe/aem-project-archetype).

## Section 1: Add the connector to existing project structure

* [Generate a local Maven repository](#generate) 
* [Update the project's POM files](#update)

### Generate a local Maven repository

Before the Workfront Connector can be included as a Maven dependency in the 'sample-site,' it must be included in a local Maven repository. The below listed steps show how to create the Workfront Connector package and include it in the 'sample-site's' source code as a repository.

#### If a repository file is provided

1. Copy the 'repository' folder and all of its contents to the root of the AEM project.

#### If a repository file is not provided and/or you're building the source code

1. In the root directory of the 'sample-site' AEM project, {sample-site-root}, create a folder called 'repository'.&nbsp;
1. In the terminal, enter the command below. Be sure to replace `{connector-root}` & `{sample-site-root}` with the correct file paths for your installation:

   <pre>mvn org.apache.maven.plugins:maven-install-plugin:2.5.2:install-file -Dfile=<span class="bold">{connector-root}</span>/all/target/workfront-aem- connector.all-1.9.0-SNAPSHOT.zip -DgroupId=com.workfront -DartifactId=workfront-aem-connector.all -Dversion=1.9.0-SNAPSHOT -Dpackaging=zip -DlocalRepositoryPath=<span class="bold">{sample-site-root}</span>/repository</pre>

1. Continue to the following section: Update the project's POM&nbsp;files.

### Update the project's POM&nbsp;files

The next step for including the Workfront Connector as a Maven dependency is to update the project POM files for the 'sample-site' AEM project. The steps below outline which POM files need to be updated and what information needs to be included.

<ol> 
 <li value="1">In the Main POM file, {sample-site-root}/pom.xml, find the 'profiles' section that includes a profile with the id 'adobe-public'.</li> 
 <li value="2"> <p>In the 'adobe-public' profile, find the 'repositories' section and include the snippet below as a new entry:</p> 
  <div class="workfront_plans"> 
   <pre><repository> <id>project.local</id> <name>project</name> <url>file:${maven.multiModuleProjectDirectory}/repository</url> </repository></pre> 
  </div> <note type="note">
   This is where the new repository entry is created for the local Maven repository created in Generate a local Maven repository section above.
  </note> </li> 
 <li value="3"> <p>In the same POM file, {sample-site-root}/pom.xml, find the 'dependencies' section and include the snippet below as a new entry:</p> 
  <div class="workfront_plans"> 
   <pre><dependency> <groupId>com.workfront</groupId> <artifactId>workfront-aem-connector.all</artifactId> <version>1.9.0-SNAPSHOT</version> <type>zip</type> </dependency></pre> 
  </div> </li> 
 <li value="4">Save the pom.xml file. Next, you need to edit the sample-site.all module's POM file to include the Workfront Connector in the deployment.</li> 
 <li value="5"> <p>In the sample-site.all module's POM file, {sample-site-root}/all/pom.xml, find the 'configuration' section under the plugin with the artifactId 'filevault-package-maven-plugin' and include the snippet below as a new entry:</p> 
  <div class="workfront_plans"> 
   <pre><embedded> <groupId>com.workfront</groupId> <artifactId>workfront-aem-connector.all</artifactId> <type>zip</type> <target>/apps/sample-site-vendor-packages/application/install</target> </embedded></pre> 
  </div> </li> 
 <li value="6"> <p>In the same POM file, {sample-site-root}/all/pom.xml, find the 'dependencies' section and include the snippet below as a new entry. This is where the Workfront Connector dependency will be added.</p> 
  <div class="workfront_plans"> 
   <pre><dependency> <groupId>com.workfront</groupId> <artifactId>workfront-aem-connector.all</artifactId> <type>zip</type> </dependency></pre> 
  </div> </li> 
 <li value="7">Save the pom.xml file.<br>Continue to Section 2: Configure the connector</li> 
</ol>

## Section 2: Configure the connector

In order for the Workfront Connector to connect to a Workfront environment, it must be configured in AEM. Because the Workfront Connector's configuration console is inaccessible in an AEM as a Cloud Service environment, the configurations must be included in the 'sample-site' AEM Project's source code. The steps below outline what configurations need to be included and where they need to be located within the 'sample-site's' source code.

1. In the Source code, navigate to the following path '{sample-site-root}/ui.apps/src/main/content/jcr_root/apps/sample-site/config'.
1. Create a file named 'com.workfront.dam.integration.config.impl.WorkfrontConfigServiceImpl.xml' in the config folder.
1. Add the snippet below as the contents of the newly created file. The `bolded` attributes should have their values customized to suit the specific implementation.

   <pre><?xml version="1.0" encoding="UTF-8"?></pre><pre><jcr:root xmlns:jcr="http://www.jcp.org/jcr/1.0"</pre><pre>xmlns:sling="http://sling.apache.org/jcr/sling/1.0"</pre><pre>jcr:primaryType="sling:OsgiConfig"</pre><pre><span class="bold">workfront.folder.path</span>="/content/dam/{PATH}"</pre><pre><span class="bold">workfront.api.key</span>="{WORKFRONT_ADMIN_USER_API_KEY}"</pre><pre><span class="bold">workfront.url</span>="https://organization.my.workfront.com"</pre><pre><span class="bold">webhooks.api.key</span>="{UNIQUE_ID}"</pre><pre><span class="bold">document.sync.auth.token</span>="{UNIQUE_ID}"</pre><pre><span class="bold">comment.sync.auth.token</span>="{UNIQUE_ID}"</pre><pre><span class="bold">metadata.sync.auth.token</span>={UNIQUE_ID}"</pre><pre><span class="bold">request.whitelist</span>="[{IP_ADDRESS_LIST}]"</pre><pre><span class="bold">ignore.domain</span>="{Boolean}false"</pre><pre><span class="bold">use.sso.username</span>="{Boolean}false"</pre><pre><span class="bold">show.collections</span>="{Boolean}true"</pre><pre><span class="bold">version.enabled</span>="{Boolean}true"/></pre>

1. The following describes each attribute and how to configure them:

  1. `workfront.folder.path`: The assets path where Workfront files are stored. This path must be within /content/dam. If changed, the new path must already exist..
  1. <![CDATA[  ]]> `workfront.api.key`: Retrieved from Customer Info section of the Workfront setup screen. This must be a Workfront admin user's API Key.
  1. `workfront.url workfront.url`: The URL of the Workfront instance being linked to. Example: https://[account].my.workfront.com
  1. The following keys and tokens can be created using the following URL to generate a unique guid for each: [UUID Generator](https://www.uuidgenerator.net/).&nbsp;

    1. `webhooks.api.key`:&nbsp;REQUIRED This will act as the AEM API key stored in the Workfront Custom configuration for the Workfront Connector.&nbsp;
    1. `document.sync.auth.token`: This auth token will create a webhook within the Workfront environment that will enable users to automatically create new proof versions of a document in Workfront when the file content is updated in AEM. If left empty, this feature will be disabled.
    1. `comment.sync.auth.token`: This auth token will create a webhook within the Workfront environment that will enable users to synchronize comments on a linked document. If left empty, this feature will be disabled.
    1. `metadata.sync.auth.token`: This auth token will create a webhook within the Workfront environment that will enable users to synchronize metadata on a linked document. If left empty, this feature will be disabled.
    1. `request.whitelist`: Restrict access to only those requests originating from the IP list specified.

      1. Input a comma separated list of whitelisted IP Addresses. Ex: [1.1.1.1,0.0.0.0]

       `<li><span class="bold">ignore.domain</span>: If enabled, the email address domain name will be ignored when mapping users from Workfront to AEM. i.e. @example.com  <ol>   <li value="1">Options: {Boolean}false or {Boolean}true</li>  </ol></li>``<li><span class="bold">use.sso.username</span>: If enabled, the connector will use the Workfront user's Federated ID when mapping users to AEM.</li>`

      1. Options: {Boolean}false or {Boolean}true

    1. `show.collections`: This option enables Workfront users to see AEM Asset Collections and link them in the Workfront Documents UI. Linked Collections cannot have documents added to them.

      1. Options: {Boolean}false or {Boolean}true

    1. `version.enabled`: This option enables Workfront users to leverage AEM Versioning when the assets already exist in DAM.

      1. Options: {Boolean}false or {Boolean}true

## Section 3: Add service user to ACLs

The 'workfront-service' user requires the following permissions to these locations:

| `Location`  | `Permission`  |
|---|---|
| > /content/dam | jcr:read rep:write |
| > /home | jcr:read |
| > /conf  |jcr:read |

A separate package with the ACLs for the 'workfront-service' service user is provided. AC Handling has been set to 'merge' so the package can be uploaded through package share to install without interfering with existing ACLs.

Please work with the customer to determine the best way to incorporate these ACLs to their environment.

## Section 4: Add Workfront metadata mapping nodes to /conf

Configurations for metadata mapping have been removed from the base package of the connector. It is recommended that these configurations are created and checked in to source control for the AEM project.

The structure should look like the following:

<pre>>/conf/global-workfront/settings/dam/adminui-extension/workfront-property-mapper</pre><pre>The primary types are:</pre><pre>> /global-workfront (sling:Folder)</pre><pre>> /settings (sling:Folder)</pre><pre>> /dam (cq:Page)</pre><pre>> /adminui-extension (sling:Folder)</pre><pre>> /workfront-property-mapper (sling:Folder)</pre>If you attempt to create a mapping without these locations pre-defined in CRX, the mapping tool will not save your configuration and instead throws an 500 error when attempting to save the mapping.

A package that contains these nodes is also available should you need it to add to your AEM project source code.

## Section 5: Integrate Workfront with AEM

After you add the connector to your existing project structure and configure the connector in AEM as described in sections 1 and 2 in this document, you must configure Workfront to link documents between&nbsp;Workfront and AEM.

<ol> 
 <li value="1"> <p>Log in to Workfront as a Workfront administrator. </p> <note type="tip">
   Workfront recommends creating a Workfront administrator dedicated solely to your AEM integration. For more information about assigning the Workfront administrator access level to a user, see 
   <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.
  </note> </li> Click the Main Menu icon in the upper-right corner of Adobe Workfront, then click Setup . 
 <li value="3">Click&nbsp;<span class="bold">Documents&nbsp;</span>>&nbsp;<span class="bold">Custom Integration.</span></li> 
 <li value="4">Click <span class="bold">Add Custom Integration</span>.</li> 
 <li value="5"> <p>In the&nbsp;<span class="bold">Name</span> box, specify the name of the custom integration.</p> <p>This is the name users see when using the integration within Workfront; for example, you could enter <em>"AEM Assets"</em> for the name.&nbsp;</p> </li> 
 <li value="6"> <p>In the&nbsp;<span class="bold">Base API URL</span> box, specify the URL for your AEM instance.</p> <p>The base API URL consists of the URL for your AEM instance followed by the path: /bin/webhooks/api/</p> <p> <img src="assets/mceclip3-350x130.png" alt="mceclip3.png" style="width: 350;height: 130;"> </p> </li> 
 <li value="7">In the&nbsp;<span class="bold">Authentication Type</span> drop-down menu,&nbsp;select <span class="bold">ApiKey.</span></li> 
 <li value="8">In the<span class="bold"> API Key</span> box, paste the AEM API Key you copied when you configured AEM Assets.</li> 
 <li value="9">Click <span class="bold">Save</span>.</li> 
 <li value="10"> <p>(Optional) Ensure the integration is marked Active.<br><img src="assets/aem-custom-integration-active-350x81.png" alt="aem_custom_integration_active.png" style="width: 350;height: 81;"></p> <p>Workfront is now configured to work with AEM Assets.</p> <p>In order to access assets in AEM, each Workfront user who needs to use the connector must be set up as a user in AEM. For information on creating users, see&nbsp;<a href="#setting" class="MCXref xref">Set up the AEM cloud connector</a>.</p> </li> 
</ol>

## Section 6: Map metadata

In order to use custom form data from Workfront inside of AEM, you must

1. Set up any custom form fields you want to use in the metadata schema in AEM. Please refer to your AEM administrator for instructions on how to set this up.
1. Once the metadata schema is in place, you must set up the Workfront Property Mapping as described in the [Set up Workfront Property Mapping](#set) section below.

### Set up Workfront Property Mapping

<ol> 
 <li value="1">In AEM, click the tool icon on the left side of the screen.</li> 
 <li value="2">Click <span class="bold">Assets</span>, then <span class="bold">Workfront Property Mapping</span>. </li> 
 <li value="3">Click <span class="bold">New Mapping</span> in the right corner of the screen.</li> 
 <li value="4">Specify the following:<br> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Workfront Field Name</td> 
     <td>Enter the name of the custom form field from Workfront.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">AEM Property</td> 
     <td>Enter the name of the metadata field previously set up in the schema.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Property Type</td> 
     <td>Select <span class="bold">String</span>. </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Property Path</td> 
     <td>This field populates automatically.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Multifield</td> 
     <td>Check the box if the field is set up as a multi-select field in Workfront.</td> 
    </tr> 
   </tbody> 
  </table></li> 
</ol>

