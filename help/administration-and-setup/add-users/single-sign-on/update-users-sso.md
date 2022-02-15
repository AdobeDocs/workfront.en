---
filename: update-users-SSO
user-type: administrator
product-area: system-administration;user-management
navigation-topic: single-sign-on-in-workfront
---



# Update users for single sign-on {#update-users-for-single-sign-on}



>[!IMPORTANT] {type="important"}
>
>The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Business Platform.
>
>
>If your organization has been onboarded to the Adobe Business Platform, Single Sign-On (SSO) is handled automatically as part of that integration. You do not need to configure or enable this functionality.
>
>
>For a list of procedures that differ based on whether your organization is migrated to Adobe IMS, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](actions-in-admin-console.md).



When single sign-on (SSO) is enabled in your *`Adobe Workfront`* instance, you can log into *`Workfront`* with your SSO credentials.


If you have an existing system that is already populated with users associated with SSO credentials, you can import the users' IDs into *`Workfront`* by importing a comma-separated values (CSV) file into *`Workfront`*.


For more information about integrating *`Workfront`* with an SSO system, see [Overview of single sign-on in Adobe Workfront](sso-in-workfront.md).


##  

## Access requirements {#access-requirements}

You must have the following to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>You must be a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For more information, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

{#access-requirements-you-must-have-the-following-to-perform-the-steps-in-this-article-adobe-workfront-plan-any-adobe-workfront-license-plan-access-level-configurations-you-must-be-a-workfront-administrator-for-more-information-see-grant-a-user-full-administrative-access-note-if-you-still-dont-have-access-ask-your-workfront-administrator-if-they-set-additional-restrictions-in-your-access-level-for-information-on-how-a-workfront-administrator-can-modify-your-access-level-see-create-or-modify-custom-access-levels}



## SSO usernames {#sso-usernames}

Depending on what SSO solution you use, the username in your SSO environment can be called any of the following:



* SSO Username
* Federation ID 
* Federation Username
* LDAP Username
* AD Username
* Active Directory Username


In *`Workfront`*, all these names are stored in the SSO Username field, on the user object. 


In order for your users to be able to use their SSO credentials to log in to *`Workfront`*, you must update their profile to include their SSO Username, in addition to their *`Workfront`* username.


As a *`Workfront administrator`*, you can bulk update the SSO Username field for your *`Workfront`* users by using a list of usernames and importing it in *`Workfront`*. This list must contain the *`Workfront`* User ID (GUID) as well as the corresponding SSO Username for each user and it must be saved as a CSV or a TSV file. This process either updates existing SSO Usernames in *`Workfront`*, or adds a new SSO Username, if one is missing for users. 


## Prepare the import file {#prepare-the-import-file}

You can start preparing your import file by building a report of all users in *`Workfront`* that must have their SSO Username fields updated.



1.  Build a user report in *`Workfront`*.


   For instructions on building user reports in *`Workfront`*, see [Create a custom report](create-custom-report.md). 

1.  Select the following fields in your report:


   ![](assets/users-with-sso-username-and-no-sso-access-only-field-350x47.png)




1. Save the report. 
1. Click `Export` at the top of the report and export the report to Excel. 
1.  Open the exported Excel file, and start adding your SSO Usernames for each user in the report in the SSO Username column.


   >[!IMPORTANT] {type="important"}
   >
   >SSO usernames are case-sensitive. 



1. Eliminate all columns in the Excel file, except for the `ID` and the `SSO Username` columns. 

1.  Eliminate the column headers and ensure there are no blank rows at the top of the report. 


   The file you are using for updating your *`Workfront`* users with the SSO usernames must contain just 2 columns, in this order:

    
    
    * The first column should display the *`Workfront`* user ID (the user GUID as found in *`Workfront`*).
    
    * The second column should contain the SSO Username, as it displays in your SSO system.
    *  The columns should have no headers, and there should not be any empty rows at the top of the list of names.
    
    
      ![](assets/update-users-for-sso-csv-file-for-import-350x47.png)    
    

    
    
    

1. Save the report as a CSV or TSV file on your computer.




## Update your users for SSO {#update-your-users-for-sso}

The process of updating users for SSO either adds the SSO Username field to your *`Workfront`* users if one is not present, or updates the value in that field if there is a value already associated with the users.



1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. Click `System` then `Update Users For SSO`.

1.  Click `Choose File` to browse for the file you prepared.


   For more information about how to prepare this file, see [Prepare the import file](#preparing-the-import-file).

1.  Select the file where it is saved on your computer, then click **Open**.


   This enables all users to log in to *`Workfront`* using their SSO credentials. 


   The `Only Allow <SSO Configuration> Authentication` setting is enabled for all users included in the CSV. For more information about user settings, see [Update users for single sign-on](#).





## Verify SSO your users' *`Workfront`* usernames {#verify-sso-your-users-workfront-usernames}

For instructions on building a user report containing SSO Username information, see [Prepare the import file](#preparing-the-import-file).



1.  Run a user report containing SSO Username information.


   Notice that the SSO Username column is populated for each user.

1. Ensure that the values for the SSO Username column match the SSO Username on your SSO server.
1.  If the SSO Username column is blank, update your users' SSO Usernames. 


   ![](assets/users-with-sso-field-updated-350x45.png)




   For instructions on updating your users for SSO, see [Update your users for SSO](#updating-users-for-sso).



