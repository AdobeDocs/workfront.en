---
filename: recalculate-project-timeline
product-area: projects
navigation-topic: manage-projects
---



# Recalculate project timelines {#recalculate-project-timelines}

Recalculating Timelines allows managers to see how forces outside of the project are impacting the project's timeline. A project's timeline refers to planned dates and projected dates.


Making changes to schedules, personnel time off, and other items outside the scope of a project do not impact the project timeline immediately. The project timeline is impacted when the timeline is recalculated. External influences do not take effect on your project until the recalculation occurs. 


This article describes the ways in which timeline recalculation happens. 


## Automatic recalculation {#automatic-recalculation}




* [Automatic recalculation of project timelines](#understanding-automatic-recalculation) 
* [Actions that trigger an automatic recalculation of project timelines](#actions-that-trigger-automatic-timeline-recalculation) 




### Automatic recalculation of project timelines {#automatic-recalculation-of-project-timelines}

By default, project timelines are automatically recalculated daily, and individual projects are automatically recalculated when the project scope changes. 


>[!NOTE]
>
>If the timeline of a project is longer than 15 years, the automatic recalculation is disabled. You can only select an Update Type of Manual for a project longer than 15 years. If you change the dates on the project to less than 15 years, you must manually recalculate your timeline one time before it is calculated automatically. 


*`Adobe Workfront`* recalculates timelines daily only for projects where all of the following conditions are met:



* Have a status of Current
*  Update Type of the project is set to Automatic or Automatic and On&nbsp;Change


  For information about the type of project Update Type, see the [Project Update Types](#project) section in this article. 

* Have a Last&nbsp;Update Date within the past three months  
  System administrators can change this default functionality, as described in [Configure timeline recalculations for projects](configure-timeline-recalculations-projects.md).

* Last calculation date of the project timeline is not within the current calendar day. This means that the last calculation date of the project timeline is before 00:00 of the current day.


You can configure how frequently the timeline for your project is updated. When the project timeline is updated, it is recalculated based on changes made to the project or changes made to another project that the timeline is dependent on.


For information, see [Select the project Update Type](select-project-update-type.md). 


### Actions that trigger an automatic recalculation of project timelines {#actions-that-trigger-an-automatic-recalculation-of-project-timelines}

Various actions automatically recalculate the timeline of a project, including:



* Updating task status.
* Moving a task to a different project.
*  Updating the Planned Date or Planned Completion Dates of the tasks. 
*  Updating the Duration Type, Task Constraint, or the number of assignees on the tasks. 
*  Updating task predecessor relationships. 
*  Adding an approval to a task that also adds time to the Planned Completion Date of the task.   
  For more information about approval settings, see [Configure global approval settings](establish-approval-settings.md).





## Manual recalculation {#manual-recalculation}

Project owners can manually recalculate the timelines for their individual projects. The *`Workfront administrator`* can manually recalculate all timelines in *`Workfront`*.



* [Recalculate timelines for individual projects](#recalculating-timelines-for-individual-projects) 
* [Recalculate timelines for the entire Workfront instance (Workfront administrators only)](#recalculating-timelines-for-the-entire-workfront-site) 




### Recalculate timelines for individual projects {#recalculate-timelines-for-individual-projects}

To recalculate the timeline for a single project:



1. Go to the project for which you want to recalculate the timeline.
1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">More</span> icon  <img src="assets/qs-more-menu.png"> in the upper-right corner, then click  <span class="bold">Recalculate Timeline</span>. </MadCap:conditionalText>`  
  
  
   After the timeline is recalculated, you see a message indicating that the recalculation was successful.  
   Before the timeline recalculation is finished, some planned or projected dates might display as dimmed. This means that the recalculation is not yet finished, and the dates are subject to change.





### Recalculate timelines for the entire *`Workfront`* instance ( *`Workfront administrators`* only) {#recalculate-timelines-for-the-entire-workfront-instance-workfront-administrators-only}

*`Workfront administrators`* can run the Recalculate Timeline diagnostic to immediately recalculate all timelines in the *`Workfront`* system. This allows all Project Managers to see the influence of external changes immediately on both planned and projected dates.


For more information about recalculating timelines for the entire *`Workfront`* site, see the section "Recalculate timelines for the entire *`Workfront`* instance" in [Configure timeline recalculations for projects](configure-timeline-recalculations-projects.md).


## Project Update Types {#project-update-types}

For information about how to update the project's Update Type, see [Select the project Update Type](select-project-update-type.md). 


>[!IMPORTANT] {type="important"}
>
>If the timeline of a project is longer than 15 years, *`Workfront`* does not calculate the timeline automatically or on change. The Update Type of a project longer than 15 years is always Manual. 


You can select how each project calculates its timeline by choosing between the following Update Types:



*  `Automatic and On Change:`&nbsp;This is the default setting. The project timeline is updated each time a change occurs&nbsp;in the project or in another project that the timeline is dependent on. The project timeline is also updated each night.&nbsp;   
  This is the recommended setting as it ensures that the project timeline is always up to date.


  When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed. 


  ![](assets/dates-dimmed-when-insline-editing-350x146.png)




  This indicates that the recalculation is not yet finished, and the dates are subject to change. 

* `Change Only:`&nbsp;The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur.   
  You might want to select this option if you are concerned about system performance and if&nbsp;changes rarely occur in the project or in other projects that the timeline is dependent on.

*  `Automatic Only:`&nbsp;The project timeline is updated each night; it is not updated immediately after changes are made.  
  You might want to select this option if you are concerned about system performance and if many changes occur each day in the project or in other projects that the timeline is dependent on.


  >[!NOTE]
  >
  >A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change.



* `Manual Only:` The project timeline is updated only when you select the option to `Recalculate Timelines`, as described in the section "Manual Recalculation" in&nbsp;the article [Recalculate project timelines](#).  
  You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).



