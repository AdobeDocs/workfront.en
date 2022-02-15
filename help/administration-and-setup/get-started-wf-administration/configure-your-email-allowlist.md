---
filename: configure-your-email-allowlist
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
---



# Configure your email allowlist {#configure-your-email-allowlist}

If your organization uses the *`Workfront`* *`Enterprise`* plan, you can create a *`Workfront`* email allowlist to control:



* Which email domains are allowed to accept emails from *`Workfront`*.
* Which email domains can be in the email address that users specify in their user profile.


This is useful if your organization’s security policy restricts users from sending data stored in *`Workfront`* to external email addresses—you can include only your internal company domains in the allowlist to ensure that this policy is followed.


>[!IMPORTANT] {type="important"}
>
>*Your IT team* should ensure that incoming email from >
>
>```>
>notifications@my.workfront.com
>```>
>
>is not blocked in your organization’s system.
>
>
>All email from *`Workfront`* is sent from that address to increase successful email delivery and to eliminate spoofing of emails. This includes both automated alerts and user-to-user communication.
>
>
>For example, the From line in a *`Workfront`* email you receive from a user named Joan Harris would look like this:
>
>
>
>
>```>
>Joan Harris <notifications@my.workfront.com>
>```>
>




For information about configuring your organization's firewall to open communication between your environment and the *`Adobe Workfront`* servers, see [Configure your firewall](configure-your-firewall.md).


## Access requirements {#access-requirements}

You must have the following to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
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



## Configure your email allowlist {#configure-your-email-allowlist-1}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. Click `System` > `Customer info`.

1.  In the `Email Allowlist` section, select `Enable Domain Allowlist`, then click `Add Domain`.
1. In the box that displays, type a domain that you want to allow, such as 

   ```
   ourcompany.com
   ```

   , then click `Add Domain`.

1. Repeat the previous step to add any other domains you want to allow.
1. When you are finished, click `Save`.


