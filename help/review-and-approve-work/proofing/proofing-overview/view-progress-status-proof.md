---
filename: view-progress-status-proof
product-area: documents
navigation-topic: manage-proofs-within-workfront
---



# *`Proof`* progress and status overview {#proof-progress-and-status-overview}

You can view information about how a *`proof`* is progressing through the review process and see an overall summary of the proof's decision status from the Documents area. 


## *`Proof`* progress overview {#proof-progress-overview}

Proof progress indicates the work done on a *`proof`* from the time you send the *`proof`* to recipients to the time they make a decision on the *`proof`*. The progress icons, S, O, C, and D, appear next to the *`proof`* name and provide information about the proof's progress.


![](assets/proof-edit-existing-progress-350x62.png)



<table style="height: 532px;margin-left: 0;margin-right: auto;width: 568;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <td class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"> <p><span class="bold">Progress icon</span> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"> <p><span class="bold">Description</span> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p> <img src="assets/proof-progress-sent-icon.png" alt=""> </p> <p><span class="bold">Sent</span> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> has been sent to assigned recipients.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p><span class="bold"><img src="assets/proof-progress-opened-icon.png" alt=""></span> </p> <p><span class="bold">Opened&nbsp;</span> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>All assigned recipients open&nbsp;the <span class="mc-variable WFVariables.proof-v variable varname">proof</span> or Proof details page.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p><span class="bold"><img src="assets/proof-progress-comment-icon.png" alt=""></span> </p> <p><span class="bold">Comments made</span> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>All assigned recipients make at least one comment on the <span class="mc-variable WFVariables.proof-v variable varname">proof</span>.</p> <p>If there are no reviewers&nbsp;assigned to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>, the <span class="bold">C</span>&nbsp;icon does not appear in the progress bar.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"> <p> <img src="assets/proof-progress-decision-icon.png" alt=""> </p> <p><span class="bold">Decision made</span> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>All assigned approvers make a decision on the <span class="mc-variable WFVariables.proof-v variable varname">proof</span>, All assigned approvers make a decision on the proof, unless the proof creator specifies only one decision is needed.</p> <p>If there are no approvers (decision makers) designated for&nbsp;the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>,&nbsp;the <span class="bold">D</span>&nbsp;icon does not appear in the progress bar.&nbsp;</p> </td> 
  </tr> 
 </tbody> 
</table>

The progress icons can appear in the following colors to indicate certain information about the *`proof`*'s progress:



* `Green`: Complete.
* `White`: Not complete.
* `Orange`:&nbsp;Not&nbsp;complete and deadline is less than 24 hours. 
* `Red`: Not&nbsp;complete and past the deadline.




## Proof status overview {#proof-status-overview}

The *`proof`* status displays the status of decisions that are required for the *`proof`*. The status of the *`proof`* is driven by the “worst case” participant. For example, suppose there are three decisions on the *`proof`*: two have the status of `Accepted` and one has the status of `Rejected`. The "worst case" decision of `Rejected` over-rules the other decisions and the overall status of the *`proof`* is shown as `Rejected`.&nbsp;


![](assets/proof-edit-existing-progress-350x62.png)




The standard status options are as follows:



* Pending
* Approved
* Approved with Changes
* Changes Required
* Not Relevant


If custom decisions are configured in your account, the status options reflect your&nbsp;custom decision&nbsp;settings.
