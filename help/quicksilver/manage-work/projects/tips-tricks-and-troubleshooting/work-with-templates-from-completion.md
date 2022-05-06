---
filename: work-with-templates-from-completion
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Work with templates scheduled from Completion
description: (drafted this article because I added this information in this article instead: /Content/Manage work/Projects/Create and Manage templates/overview-of-start-completion-day-on-template.htm)
hidefromtoc: true
---

# Work with templates scheduled from Completion

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(drafted this article because I added this information in this article instead: /Content/Manage work/Projects/Create and Manage templates/overview-of-start-completion-day-on-template.htm)</p>
-->

Consider the following when working with templates scheduled from Completion Date:

* Changing the Start Day sets the Task Constraint to Must Start On.
* Changing the Completion Day sets the Task Constraint to Must Finish On.
* When the template is scheduled from&nbsp;Completion Day, the Task Constraint Day is calculated from the Completion Day.

  ``` ```**Example: **``````Your template's duration is 285 days, and you have a template task with duration 60 days. If you set the Task Constraint to Must Start On and Constraint Day to 120, you will end up with Start Day 165 (285 - 120) and Completion Day 225 (165 + 60). So&nbsp;when you edit the Start Day, it is actually being interpreted as Constraint Day.

