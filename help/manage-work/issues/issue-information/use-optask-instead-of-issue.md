---
filename: use-optask-instead-of-issue
product-area: projects
navigation-topic: issue-information
---



# Use "opTask" and "issue" when referencing issues {#use-optask-and-issue-when-referencing-issues}

The name of an issue appears as 

```
opTask
```

in the *`Adobe Workfront`* database. Although there are times when you need to use the 

```
issue
```

field name for issues, most of the time you must use the 

```
opTask
```

field name instead of 

```
issue
```

when referencing issues. 


For more information about how objects appear in the *`Workfront`* database, refer to the [API Explorer](https://one.workfront.com/s/api-explorer). 


## Use 

```
optask
```

{#use-optask}

Use the 

```
opTask
```

reference to issues in the following contexts:&nbsp;



* When you create a text mode custom report for issues, and you want to reference issues in views, filters, groupings, or prompts.  
  For more information about using text mode in a report, see [Text Mode overview](understand-text-mode.md).

* When you pull information about issues using our API.  
  For more information about the *`Workfront`* API, see [Adobe Workfront API](workfront-api.md)

* When you update issue fields in a Kick-Start data importer sheet.  
  For more information about importing data in *`Workfront`* using a Kick-Start, see [Import data into Adobe Workfront via a Kick-Start template](import-data-via-kickstarts.md).





## Use 

```
issue
```

{#use-issue}

Use the 

```
issue
```

reference in the following contexts:



*  When you reference issues in a collection using text mode in a report. 
*  When you reference an issue collection using the *`Workfront`* API. 


For information about reporting on collections, see [Reference collections in a report](reference-collections-report.md). 
