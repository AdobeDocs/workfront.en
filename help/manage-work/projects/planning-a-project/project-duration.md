---
filename: project-duration
content-type: overview
product-area: projects
navigation-topic: plan-a-project
---



# Overview of project Duration {#overview-of-project-duration}

*`Adobe Workfront`* calculates the Duration of a project by taking into account the Start Date of the earliest task and the Completion Date of the latest task and counts the number of days between the two dates.&nbsp;


## Project Duration {#project-duration}

The Duration of the project is calculated by the following formula:




```
Project Duration = Completion Date of the latest task - Start Date of the earliest task
```




>[!NOTE]
>
>The Duration of issues on the project does not affect the Duration of the Project.




##  

The duration of the project counts the number of days between the two task dates based on the Schedule associated with the project or the users assigned to the tasks. For information about which schedule *`Workfront`* uses to calculate duration, see [Schedules overview](schedules-overview.md). 


## Types of project Duration {#types-of-project-duration}

There are two types of Project Duration and the formulas by which  *`Workfront`* calculates them:



* `Planned Duration`:&nbsp;

  ```
  Project Planned Duration = Planned Completion Date of the latest task - Planned Start Date of the earliest task / Typical hour per day
  ```


* `Actual Duration`:&nbsp;

  ```
  Project Actual Duration = Actual Completion Date of the latest task - Actual Start Date of the earliest task / Typical hour per day
  ```






## Locate the project Duration {#locate-the-project-duration}

You can locate the Project Planned and Actual Durations in the following areas of *`Workfront`*:



*  .`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">  In the Project Details area, in the Overview section. </MadCap:conditionalText>`


  For more information about the Overview sub-tab of a project, see the article [Manage information in the project Overview area](understand-project-overview-area.md).

*  In a Project report, by including the Duration or the Actual&nbsp;Duration fields in the report.


  For more information about creating reports, see the article [Create a custom report](create-custom-report.md).



