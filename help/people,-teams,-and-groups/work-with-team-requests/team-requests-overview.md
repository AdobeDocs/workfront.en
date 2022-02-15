



# Team Requests overview {#team-requests-overview}



## Understand Team Requests {#understand-team-requests}



>[!NOTE]
>
>Agile teams do not have team requests.


The Team Requests tab&nbsp;shows the requests awaiting assignment for the team that is currently selected in the drop-down list. The number in parentheses indicates how many items are ready to be worked on.


A Team Request represents a pending work item that is not assigned to a specific user. Instead, it is assigned to a team, and any member of that team can volunteer to accept responsibility for the item. If a user volunteers to work on a Team Request, the user is accepting the work assignment as their own. The task is assigned to the individual user in addition to the team.




>[!NOTE]
>
>A&nbsp;Team Request should not be used for collaborative task assignments. If you need to assign multiple users to work together on a task, do this through Advanced Assignments and not through Team requests. For more information, see [Create advanced assignments](create-advanced-assignments.md).


  



## Understand&nbsp;the Ready to Start and All Subtabs {#understand-the-ready-to-start-and-all-subtabs}

The Ready to Start `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> option </MadCap:conditionalText>`shows only tasks and issues that meet all of the following criteria:



* All predecessors have met the&nbsp;conditions for their&nbsp;predecessor dependency types.  
  For example, if the type of predecessor relationship is&nbsp;Finish-Start (predecessor task must finish before the dependent task can start), the predecessor must be&nbsp;marked as Complete.(For more information about predecessor dependency types, see [Overview of task dependency types](task-dependency-types.md).)

* The logged-in user&nbsp;is the person assigned to these tasks and issues (for Work Requests). Or the selected team is assigned to these tasks and issues (for Team Requests).
* The project status is in a status of Current.
* The Projected Start Date or Planned Start Date has passed or is scheduled to begin within 2 weeks from today's date (or no Projected Start Date or Planned Start Date&nbsp;has been defined).
* The&nbsp;Handoff Date has already occurred or will occur within 2 weeks from the current date.


The&nbsp;All`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> option </MadCap:conditionalText>`shows all tasks and issues on current projects that are assigned to the logged-in user or all tasks or issues assigned to the team.
