---
filename: project-owners-and-sponsors
content-type: overview
product-area: projects;user-management
navigation-topic: plan-a-project
---



# Overview of project owners and sponsors {#overview-of-project-owners-and-sponsors}

You can designate a Project&nbsp;Owner and a Project Sponsor for a project. 


The Project Owner is the individual responsible for the completion of the project on time and on budget. 


The Project Sponsor is an important stakeholder for the project that has resources invested in the project. The project's completion typically benefits the Project Sponsor. 


For information about how to update the Project Owner or Sponsor for a project, see [Update project owners and sponsors](update-project-owners-and-sponsors.md).


## Project owners {#project-owners}

You can designate the manager of a project by specifying a Project Owner on a project or a template.&nbsp;


You can define only one Project Owner for a project.&nbsp;


The following are possible using the Project Owner field:&nbsp;



*  You can designate only one user as the Project&nbsp;Owner. 
* You can designate Project Owners as the hours approver for the project.
*  You can designate the Project Owner as a generic approver when defining project, task, or issue approvals processes. For information about approvals, see [Edit an approval process](edit-an-approval-process.md). 


  >[!IMPORTANT] {type="important"}
  >
  >When you assign an approval to the Project Owner and no one is designated as the owner of a project, the approval is the approval is reassigned to the *`Workfront administrator`*.   




*  You can enable certain notifications that are delivered only to the Project Owner.


  For more information about email notifications, see the section [Configure event notifications for everyone in the system](configure-event-notifications-for-everyone-in-the-system.md#modify) in the article [Configure event notifications for everyone in the system](configure-event-notifications-for-everyone-in-the-system.md).

*  You can display the Project Owner field in a report or list. 


  You can also display the Project Owner field in a view, grouping, or prompt.


  For example, you can copy the following text mode expression into a filter to display projects owned by the logged in user:&nbsp;

  ```
  ownerID=$$USER.ID
  ```

  &nbsp;


  For more information about creating reports, see the article [Create a custom report](create-custom-report.md).





## Project sponsors {#project-sponsors}

You can designate any user in the system as a Project Sponsor.&nbsp;The Project Sponsor is usually a manager, executive, or stakeholder who needs to know what is happening with the project.


Consider the following when assigning a Project Sponsor:



*  The Project Sponsor does not&nbsp;gain&nbsp;any additional access to the project but is added to the email notifications of the project. For information about notifications, see the article [Configure event notifications for everyone in the system](configure-event-notifications-for-everyone-in-the-system.md).





*  You can designate only one Project Sponsor.
*  You can designate the Project Sponsor as a generic approver when defining project, task, or issue approvals processes. For information about approvals, see [Edit an approval process](edit-an-approval-process.md). 


  >[!IMPORTANT] {type="important"}
  >
  >When you assign an approval to the Project Sponsor and no one is designated as the sponsor of a project, the approval is assigned to the Project Owner, by default. If no one is designated as the owner of the project, the approval is assigned to the *`Workfront administrator`*.   




*  You can display the Project&nbsp;Sponsor field in a report or list.


  You can also display the Project Sponsor field in a view, grouping, or prompt.


  For example, you can copy the following text mode expression into a filter to display projects sponsored by the logged in user:&nbsp;

  ```
  sponsorID=$$USER.ID
  ```

  &nbsp;


  For more information about creating reports, see the article [Create a custom report](create-custom-report.md).



