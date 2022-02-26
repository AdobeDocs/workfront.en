---
filename: earliest-available-time
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: Task Constraint overview: Earliest Available Time
description: Earliest Available Time is a Task Constraint that schedules a task to begin at the earliest available time after considering any predecessor relationships.
---

# Task Constraint overview: Earliest Available Time

Earliest Available Time is a Task Constraint that schedules a task to begin at the earliest available time after considering any predecessor relationships.

For information about how to update the Task&nbsp;Constraint on a task, see [Update the Task Constraint of a task](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To update the Task Constraint to Earliest Available Time:</p>
-->

To update the Task Constraint to Earliest Available Time:

<ol> <draft-comment>
  <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Go to a task whose constraint you want to modify. </li>
 </draft-comment>
 <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Go to a task whose constraint you want to modify. </li> 
 <li value="2"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <span class="bold">Edit Task</span>.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <span class="bold">Edit Task</span>.</p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the <span class="bold">More</span> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <span class="bold">Edit</span>.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the <span class="bold">More</span> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <span class="bold">Edit</span>.</p> </li> 
 <li value="3"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <span class="bold">Overview</span> section, expand the <span class="bold">Task Constraint</span> drop-down menu.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <span class="bold">Overview</span> section, expand the <span class="bold">Task Constraint</span> drop-down menu.</p> </li> 
 <li value="4"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Select <span class="bold">Earliest Available Time</span>.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">Select <span class="bold">Earliest Available Time</span>.</p> </li> <draft-comment>
  <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <span class="bold">Save Changes</span>.</li>
 </draft-comment>
 <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <span class="bold">Save Changes</span>.</li> 
</ol>

## The difference between Earliest Available Time and As Soon As Possible

The Earliest Available Time constraint differs from the As Soon As Possible constraint when all of the following criteria exist:

* The project is scheduled From Completion 
* Tasks in the project have a predecessor relationship 
* The predecessor task has a flexible task constraint

In this situation:

<ul> 
 <li> <p><span class="bold">Earliest Available Time:</span> Using the Earliest Available Time constraint on the successor task gives priority to the predecessor's flexible constraint.</p> 
  <div class="example" data-mc-autonum="<b>Example: </b>">
   <span class="autonumber"><span><b>Example: </b></span></span> 
   <p>Task A is a predecessor to Task B. Task B has the Earliest Available Time constraint and Task A has the As Late As Possible constraint. In this situation, Task B is scheduled as close to the completion of the project as possible.</p> 
   <p> <img src="assets/earliest-available-constraint-dates-closer-to-project-completion-350x137.png" alt="Earliest Available Time constraint when task has the dates close to the project's Completion Date" style="width: 350;height: 137;"> </p> 
  </div> </li> 
 <li> <p><span class="bold">As Soon As Possible:</span> In this scenario, using the As Soon As Possible constraint on the successor task gives the priority to the successor task.</p> 
  <div class="example" data-mc-autonum="<b>Example: </b>">
   <span class="autonumber"><span><b>Example: </b></span></span> 
   <p> Task A is a predecessor to Task B. Task B has the As Soon As Possible constraint and Task A has the As Late As Possible constraint. In this situation, Task B is scheduled as close to the start of the project as possible.</p> 
   <p> <img src="assets/as-soon-as-possible-dates-closer-to-project-start-350x126.png" alt="As Soon As Possible constraint when task has the dates close to the project's Start Date" style="width: 350;height: 126;"> </p> 
  </div> </li> 
</ul>

