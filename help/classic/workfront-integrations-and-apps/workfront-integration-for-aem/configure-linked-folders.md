

# ```Workfront Tools for AEM User Guide : Configure Linked Folders```  {#title-heading}

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Adobe Workfront license*</td> 
    <td> <p>Plan or higher</p> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>You must have a license to Adobe Experience Manager</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>You must have access to the document folders you want to link</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

* You must install Workfront Tools for Adobe Experience Manager before you can use it to configure linked folders.

  For instructions, see [Workfront Tools for AEM User Guide: Installation Guide 1.x.x](../../workfront-integrations-and-apps/workfront-integration-for-aem/installation-guide.md)

## Configuration

1. Event Subscriptions configuration

   1. Go to the ```Event Subscriptions``` tab in the cloud services.
   1. Select the ```custom integration``` you created in Workfront.
   1. Click ```Enable Workfront Event Subscriptions```.

1. Linked folder structure configuration

   1. Go to the ```Project Linked Folders``` tab in the cloud services.
   1. Linked folder parent path: Select a folder in the DAM where you wish to create the linked folders. If left empty, it will default to /content/dam. Make sure that the ```Workfront Tools```metadata schema and ```Workfront Linked Folder``` folder metadata schema have been applied to the selected folder.
   1. Linked folder structure: Enter comma-separated values. Each value should be DE:<some-project-custom-form-field>, Portfolio, Program, Year, Name, or some "Literal String Value" (this last one with quotation marks). It is currently set to   
   
      ```   
      Portfolio,Program,Year,DE:Project Type,Name
      ```   
   
      .
   1. ```Build linked folder title in Workfront using the folder structure names``` checkbox should be checked if the title of the folder in Workfront should include all folders in the structure. Otherwise, it will be the title of the last folder.
   1. Sub-folders multifield allows specifying a list of folders that should be created as a child folder of the linked folder.
   1. Project status: Select the status the project has to be set to in order to create the linked folder.
   1. Create a linked folder in projects with portfolio: List of Portfolios that the project has to belong to in order to create the linked folder. Leave this list empty to create the linked folder for all project portfolio.
   1. Create a linked folder in projects with custom form field: Custom form field and its corresponding value that the project has to have in order to create the linked folder. This configuration will be ignored if left empty. Select ```CUSTOM FORMS: Create DAM Linked Folder```” for the field and type ```Yes```for the value.
   1. Click on ```Enable automatic creation of linked folders```. If you go back to the ```Event Subscriptions``` tab, you'll see there is now one ```create```event.

## Linked folder creation {#configurelinkedfolders-linkedfoldercreation}

1. Go to ```Projects```in Workfront and click on ```+ New Project```. Enter a name for your project.
1. At this point, if you reload the cloud services page, you'll see that there are now 3 active subscriptions:

   1. For the creation of new projects.
   1. For updates in the project that you just created.
   1. For the case where you delete the project that you just created.

1. Go to ```Project Details``` tab of the new project and to ```Custom Forms``` sub-tab.
1. Select ```Workfront Tools Project``` form.
1. Edit it and select values for ```Project Type```, ```Project Tags``` and ```Project asset types```. Select ```Yes```for ```Create DAM Linked Folder```. Leave AEM Folder URL empty (it will be populated later by an AEM workflow).
1. Also in ```Project Details``` tab, go to ```Portfolio```sub-tab and add ```Default Portfolio```. Also set the Program to ```Test Program```.
1. Change the project status to whatever you selected in the configuration.
1. At this point, if you reload the cloud services page, you'll see that ```update```and ```delete```events are no longer there for your project. These events subscriptions are deleted once they are no longer useful
1. In your Workfront project, if you go to the ```Documents```tab, you'll see the linked folder with name ```<Portfolio>-<Program>-<Project Name>-Deliverables``` or just ```Deliverables```(depending on the option for the checkbox in the cloud services).
1. You can try uploading documents into this folder or its sub-folder and check that the folder together with its content exists in AEM. Also check that the assets in AEM are identified with a small Workfront icon.
1. You should also check that the linked folder and the assets that were sent have project metadata in their properties.

   ![](assets/project-linked-folders-350x257.png)

