---
filename: create-tasks-and-issues-from-slack
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
---



# Create tasks and issues from Slack {#create-tasks-and-issues-from-slack}

After you have installed and configured *`Adobe Workfront`* for Slack, you can create tasks and issues from Slack and associate them with projects in *`Workfront`*.


For more information about configuring *`Workfront`* with Slack, see [Configure Adobe Workfront for Slack](configure-workfront-for-slack.md).&nbsp;


You must have access to create tasks and issues in your Access Level and you must have Contribute permissions on the project that you are associating them with.&nbsp;


For more information about Access Levels, see [Access levels overview](access-levels-overview.md). For more&nbsp;information about permissions to objects, see [Overview of sharing permissions on objects in Adobe Workfront](sharing-permissions-on-objects-overview.md).



## Access requirements {#access-requirements}

You must have the following:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 </col> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 </col> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader"><a href="https://www.workfront.com/plans" target="_blank"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan</a>*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Pro or higher</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.\


## Prerequisites {#prerequisites}

Before you can create tasks and issues from Slack, you must



* Configure *`Workfront`* for Slack  
  For instructions on configuring *`Workfront`* for Slack, see [Configure Adobe Workfront for Slack](configure-workfront-for-slack.md).





## Create tasks from Slack {#create-tasks-from-slack}




1.  Log in to your Slack instance and log in to *`Workfront`* from Slack.  
   For more information about logging in to *`Workfront`* from Slack, see the "Logging In to *`Workfront`* from Slack" section in [Access Adobe Workfront from Slack](access-workfront-from-slack.md).

1.  From any channel, start typing the following command in the message field:&nbsp;  
   *

   ```
   /workfront add task <Task Name>
   ```

   .*


   >[!NOTE]
   >
   >Commands are case sensitive. You can start your command with    >
   >
   >```   >
   >/wf
   >```   >
   >
   >instead of /   >
   >
   >```   >
   >workfront
   >```   >
   >
   >.  
   >The Task Name must be entered as it will appear in the *`Workfront`* interface, without brackets or quotation marks.  
   >![add_task_to_project.png](assets/add-task-to-project-350x63.png)  




1. (Optional) Start typing the name of a project with which you want to associate the new task and select it when it appears in the list.  
   You receive a confirmation indicating that the task was added to the selected project.
1. (Optional) Click the name of the task in the confirmation message to open it in *`Workfront`*, in a new browser tab.




## Create issues from Slack {#create-issues-from-slack}




1.  Log in to your Slack instance and log in to *`Workfront`* from Slack.  
   For more information about logging in to *`Workfront`* from Slack, see the "Logging In to *`Workfront`* from Slack" section in [Access Adobe Workfront from Slack](access-workfront-from-slack.md).

1.  From any channel, start typing the following command in the message field:&nbsp;  


   ```
   /workfront add issue <Issue Name>
   ```

   *.*


   >[!NOTE]
   >
   >Commands are case sensitive. You can start your command with '/wf' instead of '/workfront.'&nbsp;  
   >The Issue Name must be entered as it will appear in the *`Workfront`* interface, without brackets or quotation marks.  
   >![slack_add_issue_to_project.png](assets/slack-add-issue-to-project-350x88.png)  




1. (Optional) Start typing the name of a project with which you want to associate the new issue and select it when it appears in the list.  
   You receive a confirmation indicating that the issue was added to the selected project.&nbsp;
1. (Optional) Click the name of the issue in the confirmation message to open it in *`Workfront`*, in a new browser tab.


