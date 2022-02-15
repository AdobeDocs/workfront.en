



# Manage companies {#manage-companies}

A Company is an organizational unit in `Workfront`. You can use Companies for financial planning, reporting purposes, to define permissions around objects, and to keep information confidential.


A Company can represent:



* Your own organization
* A department in your organization
* A client you work with




## Add a Company to `Workfront` {#add-a-company-to-workfront}

As a `Workfront administrator`, you can add Companies to `Workfront`. There is no limit to the number of Companies you can add. However, we recommend that you use a limited amount of Companies, because there are permissions implications linked to Companies. Too much fragmentation might interfere with users' visibility to work items.


By default, the Company associated with your instance of `Workfront` is already created in your `Workfront` system and it is the primary Company . Your Company has the same name as your customer name. For more information about your customer information in `Workfront`, see [Configure basic info for your system](configure-basic-info.md).


To add a new Company:



1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of `Workfront`, then click **Setup** ![](assets/setup-gear-icon.png).

1.  Click **Companies**. 
1.   Click **New Company**.
1.  Specify the following information in the **New Company**&nbsp;form.

    
    
    *  In the **Basic Info** section:
    
    
    <table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Company Name</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Type a name for the Company.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">This is the Primary Company</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Select this checkbox if you want to designate this as your primary Company. The primary Company typically represents&nbsp;your <span class="WFVariablesProdNameWF">Workfront</span> account where most of your users work.</p> 
    <ul> 
     <li value="1">By modifying their access levels, you can restrict users to see only users:<br></li> 
     <li value="2">In their Primary Company</li> 
     <li value="3"> <p>In their associated&nbsp;company and the Primary Company<br></p> <p>For information about the primary Company functionality within users' access levels, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify access levels</a>. </p> <p>You can&nbsp;have only one or no Company designated as a primary Company, but you cannot have multiple Companies designated as primary Companies.&nbsp;<a href="create-modify-access-levels.md" class="MCXref xref">Create or modify access levels</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray">Company Members</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Add existing users to the Company. By doing this, you are associating these users with this Company. There is no limit to how many users you can add to a Company.<br></p> <p>For information about associating users and&nbsp;Companies, see <a href="#associating-users-with-companies" class="MCXref xref">Associate users&nbsp;with&nbsp;Companies</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>    
    
    
    
    

    
    
    *  In the **Billing Rates** section:
    
    
      You can override billing rates associated with your job roles at the Company level. For information about creating job roles and associating them with billing rates, see [Create and manage job roles](create-manage-job-roles.md).  
      For more information about overriding billing rates at the company level, see [Override job role billing rates at the company level](override-job-role-billing-rates-company-level.md).
    
    *  In the** Custom Forms** section: 
    
    
      If there are fields that you want to add to your Company that are not available in `Workfront`, you can build a Custom Form and&nbsp;associate it with your Company. You can attach this form to your Company by selecting it from the drop-down menu.&nbsp;Only active companies are listed in the drop-down menu. For information about creating Custom Forms, see [Create a Custom Form](create-a-custom-form.md). 
    
    
    

1. Click **Create Company**.&nbsp;




## Associate users, templates, and projects with Companies {#associate-users-templates-and-projects-with-companies}

You can associate a Company with both users, projects, and templates.&nbsp;


### Associate users&nbsp;with&nbsp;Companies {#associate-users-with-companies}

A user cannot be associated with more than&nbsp;one Company.  
There is no limit to how many users you associate with one Company.&nbsp;


#### Benefits of associating a user with a Company {#benefits-of-associating-a-user-with-a-company}




* You can build a&nbsp;Company's&nbsp;organization chart by associating users with direct reports. Only users from the same Company can be added as direct reports of another user from that Company.&nbsp;
* As a project manager, you can identify available resources within the same Company.
* You can keep information private between Companies by choosing one or all&nbsp;of the following settings:
*  `<li value="1">Users from the same Company can see each other's requests.&nbsp;For more information about giving similar access to requests based on users' Company, see the <a href="set-task-issue-preferences.md#changing-task-and-issue-preferences" class="MCXref xref">Change task and issues preferences</a> section in <a href="set-task-issue-preferences.md" class="MCXref xref">Task and issue preferences</a>.</li>` `<li value="2">Users can see only request queues that are associated with their Companies. For more information about&nbsp;restricting visibility of a request queue, see <a href="#associating-a-request-queue-with-a-projects-company" class="MCXref xref">Restrict the visibility of a&nbsp;request queue&nbsp;to users&nbsp;from the project's Company</a>.</li>` `<li value="3">You can restrict users to only see users in their Company or their Company and the primary Company. For information about the primary Company functionality regarding user privacy, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify access levels</a>.</li>` `<li value="4">Users can restrict updates&nbsp;they make&nbsp;on items to be visible by their Company users only. For more information about making an update private to a Company, see <a href="update-work.md" class="MCXref xref">Update work</a>.</li>` 





#### Associate a user with a Company {#associate-a-user-with-a-company}




1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of `Workfront`, then click **Users** ![](assets/users-icon-in-main-menu.png). 

1. Select an existing user, then click **Edit**.
1. Click **Organization**.
1. Select a **Company** from the drop-down menu.
1. Click **Save Changes**.




### Associate templates and projects with companies {#associate-templates-and-projects-with-companies}

A project or a template cannot be associated with more than&nbsp;one Company.  
There is no limit to how many projects or templates you associate with one Company.  



One of the benefits of associating projects with Companies&nbsp;is that you can report on project financials for each Company.&nbsp;


#### **Associate a template with a Company**  {#associate-a-template-with-a-company}

We recommend that you associate your project templates with your Companies, so you can have designated templates that are specific for each Company's projects. For more information about creating projects using a template, see [Create a project using a template](create-project-from-template.md).


To associate a template with a Company:



1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of `Workfront`, then click **Templates**. ![](assets/templates-icon-in-main-menu.png)


1. Select the template you want to associate with a Company, then click **Edit**.
1. In the **Overview** section of the **Edit Template**&nbsp;form, select a **Company** in the drop-down menu.

1. Click **Save Changes**.&nbsp;




#### **Associate a project&nbsp;with a Company**  {#associate-a-project-with-a-company}




1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of `Workfront`, then click **Projects**. ![](assets/projects-in-main-menu.png)


1. Select the project you want to associate with a Company, then click `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> the Edit icon. <img src="assets/edit-icon.png"></MadCap:conditionalText>`
1. In the **Overview** section of the **Edit Project** box, select a **Company** in the drop-down menu.

1. Click **Save Changes**.




## Restrict the visibility of a&nbsp;request queue&nbsp;to users&nbsp;from the project's Company {#restrict-the-visibility-of-a-request-queue-to-users-from-the-projects-company}

When using a project as a request queue, you can allow only users from the Company associated with this project to see the request queue in their **Requests** area of `Workfront`.


For more information about setting up a project as a request queue, see [Create a Request Queue](create-request-queue.md).



1.  Go to the project which you set up as a request queue.
1.  Ensure that the project is associated with a Company.


   For information on associating a project with a Company, see [Associate a project with a Company](#associate-a-project-with-a-company).

1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click  <b>Queue Details</b>  <img src="assets/queue-details-left-panel.png"> in the left panel.</MadCap:conditionalText>` 
1.  In the **Queue Type** section, select&nbsp;**People in this project's company**, then click **Save**.  





## About sharing objects with&nbsp;Companies {#about-sharing-objects-with-companies}

In addition to the permissions outlined in [Benefits of associating a user with a Company](#benefits-of-associating-a-user-with-a-company), you can allow users permissions to view, contribute, or edit objects in `Workfront` by sharing the object with their Company. 


Rather than sharing an object with one individual user at a time, you can share it with their entire Company. Each user in the Company has the same permissions on that object.&nbsp;


For more information about sharing objects, see [Share Permissions on objects](sharing-permissions-on-objects.md).


## Deactivate a Company {#deactivate-a-company}

You can deactivate a Company that you no longer use while retaining all of its associated historical data. If you deactivate a Company already in use somewhere in the system, it continues to function just like it always has. It will not be removed or blocked.



1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of `Workfront`, then click **Setup** ![](assets/setup-gear-icon.png).

1. In the left panel, click **Companies**. ![](assets/companies-icon-left-panel.png)


1. Select one or more Companies to deactivate.
1. Click **Edit**.
1.  If editing a single Company, select or unselect the **Is Active** box.  



   Or  



   If editing multiple Companies, select **No** from the **Is Active** drop-down menu.

1. Click **Save Changes**.


