---
filename: map-ms-project-fields-to-workfront
product-area: projects
navigation-topic: manage-projects
---



# Map Microsoft Project fields to  *`Adobe Workfront`* {#map-microsoft-project-fields-to-adobe-workfront}

Projects in *`Adobe Workfront`* and Microsoft Project are mostly compatible. Using the two applications, you can do the following:



* Export projects from Microsoft Project and import them into *`Workfront`*
* Export projects from *`Workfront`* and import them to Microsoft Project.&nbsp;


For more information about importing projects from Microsoft Project in to *`Workfront`*, see [Import a project from Microsoft Project](import-project-from-ms-project.md).


For more information about exporting a project from *`Workfront`* to import it into Microsoft Project, see [Export a project to Microsoft Project](export-project-to-ms-project.md).


When performing such imports of data, it is important to understand how information translates from one application to the other. Most times, you will have to make some manual modifications to the project, after you complete the import.&nbsp;


## Overview of field&nbsp;mapping {#overview-of-field-mapping}



>[!NOTE]
>
>Planned dates do not always correspond between both systems. Discrepancies can be accounted for through schedule and differences in system preferences between *`Workfront`* and Microsoft Project. These date discrepancies can&nbsp;also result in differences in effort, duration, and percent complete.





## Overview of data that is not included {#overview-of-data-that-is-not-included}

There are a number of project fields that are not imported to or exported from *`Workfront`*.


These fields include but are not limited to the following:



* Document attachments
* Custom fields (at the project or task levels)
* *`Workfront`* notes
* Issues
* Negative lag in tasks with a Start/ Finish predecessor relationship (tasks are imported without the lag)
* Assignments
* Task Constraints  


  >[!NOTE]
  >
  >Because Constraints do not map between Microsoft Project and *`Workfront`*, ensure that there are predecessor relationships between the tasks. Otherwise, the Planned Start and Planned Completion Dates of the tasks might not accurate in the imported project.&nbsp;





