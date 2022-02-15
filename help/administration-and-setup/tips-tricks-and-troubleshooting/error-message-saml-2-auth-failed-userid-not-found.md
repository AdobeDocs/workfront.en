---
filename: error-message-saml-2-auth-failed-userid-not-found
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
---



# Error message: SAML 2.0 Authentication Failed: User Identifier Not Found {#error-message-saml-authentication-failed-user-identifier-not-found}



## Problem {#problem}

I am receiving this error when using SAML 2.0: "SAML 2.0 Authentication Failed: User Identifier Not Found."


## Cause {#cause}

This happens when a `UID` or `NAME ID` is not passed from the `ADFS Claim rules`.&nbsp;


In ADFS the `Relying Party Trust` needs to have a `Claim rule` that passes either a `UID` or a `NAME ID` value.  When you run a ` *`Workfront`* Test Connection`, it should show this if successful.&nbsp;


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



## Solution {#solution}




1. When editing the  ` `ADFS INFO``, in the `Relying Party Trusts`> Select object > `Edit Claim Rules.`

1. The `LDAP Attribute` (left column) should have `E-Mail Addresses` (or any unique identifier).

1. The `Outgoing Claim Type` (right column) should be `Name ID`.  


   >[!NOTE]
   >
   >It does not have to have the LDAP Attribute E-Mail Addresses. Any unique identifier that will identify the user can be used but it must be passed into *`Adobe Workfront`* as the `NAME ID`.





