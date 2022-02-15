---
filename: workfront-ms-project-duration-types
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
---




# Duration Types in `Workfront` and Microsoft Project {#duration-types-in-workfront-and-microsoft-project}



## Duration Types {#duration-types}

`Workfront` has four task duration types:



* Simple
* Effort Driven
* Calculated Work
* Calculated Assignment


These duration types are not recognized by Microsoft Project. Currently, Microsoft Project has 3 task types:



* Fixed Units
* Fixed Work
* Fixed Duration 




## Export from `Workfront` {#export-from-workfront}

When exporting from `Workfront` to Microsoft Project, Effort Driven tasks become Fixed Work. Simple, Calculated Work, and Calculated Assignment become Fixed Units. 


## Import from `Workfront` {#import-from-workfront}

When importing from Microsoft Project to `Workfront`, Fixed Units become Effort Driven. Fixed Work and Fixed duration receive the default duration type.


` `**Warning: **``When a task has Calculated Work as the duration type and the default duration type in Setup is set as Calculated Assignment, then MS Project assignment allocations will be lost during the import.
