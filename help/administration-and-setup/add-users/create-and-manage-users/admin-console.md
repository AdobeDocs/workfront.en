


# Manage users in the Adobe Admin Console {#manage-users-in-the-adobe-admin-console}



>[!IMPORTANT] {type="important"}
>
>The functionality in this article is available only if your organization's instance of *`Workfront`* has been onboarded to the Adobe Business Platform.
>
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Business Platform, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](actions-in-admin-console.md).



As an Adobe administrator, you can create *`Adobe Workfront`* users and system administrators using the Adobe Admin Console. The console is a central location for managing the Adobe entitlements across your organization. For more information, see the [Admin Console Overview](https://helpx.adobe.com/enterprise/using/admin-console.html).


## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 </col> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 </col> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Adobe administrator rights</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>You must be a Product Configuration Administrator of Adobe products for your organization</p> </td> 
  </tr> 
 </tbody> 
</table>



## Prerequisites {#prerequisites}

Before using the Admin Console for Workfront, you should receive a receive an email inviting you to the console. 



1.  If you are new to Adobe and you have received an email telling you that you now have administer rights to manage Adobe software and services for your organization, click the button in the email to create an Adobe account and open the Admin Console. 


   Or


   If you already have an Adobe account, go to the [Adobe Admin Console page](https://adminconsole.adobe.com/).





## Access the user and admin area for your Production instance of Workfront {#access-the-user-and-admin-area-for-your-production-instance-of-workfront}




1.  From the [Adobe Admin Console page](https://adminconsole.adobe.com/), select the **Products** tab in the top navigation bar, and then select the **Workfront** product tile.


   ![](assets/admin-product-350x184.png)



1.  In the list that displays, select the link at the top.


   This is your Production instance where your users work. 


   ![](assets/instances-350x232.png)



   ` `**Tip: **`` Your Preview instance, the second link in the list, is a testing environment that replicates your live Production environment. For more information, see [The Adobe Workfront Preview Sandbox Environment](wf-preview-sandbox-environment.md).


   You might also see links to sandbox environments in the list. For more information, see [The Adobe Workfront Preview Sandbox Environment](wf-preview-sandbox-environment.md).

1.  In the list that displays, with the `Product Profiles` tab selected, click the name of the *`Workfront`* Product Profile link. 


   ![](assets/prod-profile-350x127.png)




   This list includes all users that are already assigned to your Production instance of *`Workfront`*. 


   >[!IMPORTANT] {type="important"}
   >
   >Do not make any changes to the Product Profile itself.



1.  Continue on to one of the following sections in this article:

    
    
    * [Create users in Workfront with the Adobe Admin Console](#create) 
    * [Create system administrators in Workfront with the Adobe Admin Console](#create2) 
    
    





## Create users in *`Workfront`* with the Adobe Admin Console {#create-users-in-workfront-with-the-adobe-admin-console}




1. Go to the user and admin area in the Admin Console, as described in [Access the user and admin area for your Production instance of Workfront](#access) in this article.
1.  With the `Users`tab selected above the list, select **Add User**.
1.  In the **Add users to this product profile** box, enter the email address or name of a user you want to add, then select **Save**. 


   The user is created in *`Workfront`* with the Requestor access level. 


   >[!IMPORTANT] {type="important"}
   >
   >Do not make any changes to the Product Profile itself.



1.  In *`Workfront`*, change the user's access level.


   For instructions on how a *`Workfront administrator`* can change the user's access level, see [Edit a user's profile](edit-a-users-profile.md).

1.  Repeat steps 3 and 4 to add more users.




## Create system administrators in *`Workfront`* with the Adobe Admin Console {#create-system-administrators-in-workfront-with-the-adobe-admin-console}

The System Administrator access level is granted only on the Adobe Admin Console. You cannot grant or remove admin access from within *`Workfront`*.


You must add a user to your Production instance of *`Workfront`* before you can make the user a *`Workfront`* system administrator. For instructions, see [Create users in Workfront with the Adobe Admin Console](#create) in this article.



1. Go to the user and admin area in the Admin Console, as described in [Access the user and admin area for your Production instance of Workfront](#access) in this article.
1.  Select the **Admins** tab above the list of users. 
1.  Select **Add Admin**.
1.  In the **Add product profile administrators** box, enter the email addresses or names of the administrators you want to add, then select **Save**. 


   ![](assets/add-admin-350x124.png)




   The system administrators are created in *`Workfront`*.


   >[!IMPORTANT] {type="important"}
   >
   >Do not make any changes to the Product Profile itself.







## Additional details about the Adobe Admin Console: {#additional-details-about-the-adobe-admin-console}




*  Workfront System Administrators can deactivate a Workfront user from within *`Workfront`*, but this does not deactivate the user in the Admin Console.
*  The user **Home Group** is determined based on the user who created them. This is currently not customizable from within the Admin Console.
*  The Workfront System Administrator access level can only be edited from within the Adobe Admin Console.
*  Editing a user who is a system admin to any other access level must be done through the Admin Console first. 
*  To remove System Administrator access from a user in *`Workfront`*, you need to use the Adobe Admin Console to remove the user as Product Profile Administrator. This changes the user's *`Workfront`* access level from System Administrator to Requestor.
*  

  >[!IMPORTANT] {type="important"}
  >
  >Do not make any changes to the Product Profile itself.




