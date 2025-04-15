---
content-type: api
navigation-topic: api-navigation-topic
title: What's new in API version 20
description: Adobe Workfront released API version 20 on April 6, 2022. API version 20 features the following changes from version 19.
author: Becky
feature: Workfront API
role: Developer
---
# What's new in API version 20

Adobe Workfront released API version 20 on April 8, 2024. API version 20 features the following changes from version 19.

## Added resources

### AssignmentBillingRole (ASBLRL)



### StaffingPlan (STAFFP)



### StaffingPlanResource (STAFFR)




## Removed resources

No resources were removed for API version 20

## Modified resources

### AccessLevelPermissions (ALVPER)

An AccessLevelPermissions object represents a specific permission to access, create, or modify a Workfront object. These permissions can then be associated with an Access Level.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b>
            </p>
            <p>Added the following possible values:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Remove from Custom Data)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Add sub-projects)</p>
              </li>
              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>
            </ul>
            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Added the following possible values:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Remove from Custom Data)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Add sub-projects)</p>
              </li>
              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>
            </ul>
            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Added the following possible values:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Remove from Custom Data)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Add sub-projects)</p>
              </li>
              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>
            </ul>
            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRequest (ACSREQ)

If a User does not have access to an object in Workfront that they need, they can request access to that object. The AccessRequest object represents this request.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>action</b>
            </p>
             <p>Added the following possible values:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Remove from Custom Data)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Add sub-projects)</p>
              </li>
              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>
            </ul>
            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRule (ACSRUL)

An AccessRule object represents a rule set in custom access levels that determines how users can share projects they create.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b>
            </p>
            <p>Added the following possible values:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Remove from Custom Data)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Add sub-projects)</p>
              </li>
              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>
            </ul>
            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Added the following possible values:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Remove from Custom Data)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Add sub-projects)</p>
              </li>
              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>
            </ul>
            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Added the following possible values:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Remove from Custom Data)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Add sub-projects)</p>
              </li>
              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>
            </ul>
            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AnnouncementAttachment (ANMATT)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>fileExtension</b>
            </p>
             <p>Added the following possible values:</p>
             <ul>
              <li>
                <p><code>tiff</code> (enum.fileextension.tiff)</p>
              </li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Approval (APPROVAL)

A given work item, such as a task, document, or timesheet, may require that a supervisor or other user sign off on the work item. An Approval object represents the action of signing off on a work item.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p>The following fields added the flag <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualBenefit</li>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualExpenseCost</li>
              <li>actualLaborCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>actualRiskCost</li>
              <li>actualValue</li>
              <li>billedRevenue</li>
              <li>budget</li>
              <li>budgetedCost</li>
              <li>budgetedHours</li>
              <li>budgetedLaborCost</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>fixedCost</li>
              <li>fixedRevenue</li>
              <li>plannedBenefit</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost</li>
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedRiskCost</li>
              <li>plannedValue</li>
              <li>remainingCost</li>
              <li>remainingRevenue</li>
              <li>remainingRiskCost</li>
              <li>resourcePlannerBudgetedHours</li>
              <li>resourcePlannerBudgetedLaborCost</li>
              <li>riskPerformanceIndex</li>
            </ul>
          </li>
          <li>
          <p>The following fields changed their type from <code>double</code> to <code>class java.math.BigDecimal</code>:
          <ul>
          <li>actualCost</li>
          <li>actualRevenue</li>
          <li>plannedCost</li>
          <li>plannedRevenue</li>
          </ul>
          </li>
          <li><p><b>plannedDuration</b></p> <p>Added the flags <code>DYNAMIC</code>, <code>LAZY_READ</code>, and <code>READ_ONLY</code></li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>Added the flag <code>CURRENCY</code></li>
          <li><p><b>costType</b></p> <p>Added the possible value <code>URH</code> (User and Role Hourly) </li>
          <li><p><b>revenueType</b></p> <p>Added the possible values <code>URH</code> (User and Role Hourly), <code>URC</code> (User and Role Hourly w/Cap), and <code>URF</code> (User and Role Hourly Plus Fixed)</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collections fields</td>
      <td>
          <p>The following fields were added:</p>
             <ul>
              <li><b>billingRates</b></li>
              <li><b>costRates</b></li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>

### Assignment (ASSGN)

An Assignment object represents the connection between a work item and the user, team, or group that is assigned to work on it.

The Assignment object added the flags `ATTRIBUTE_ATTACHABLE` and `DOMAIN_EXTENDABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>isBillable</b>
            </p>
             <p>Added</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
             <p>Added the following fields:</p>
             <ul>
              <li><b>assignmentBillingRoles<b></li>
              <li><b>billingRates<b></li>
              <li><b>costRates<b></li>
            </ul>
      </td>
   <tr>
      <td role="rowheader">Default fields</td>
      <td>
        <ul>
          <li>
            <p><b>isBillable</b>
            </p>
             <p>Added</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

### Avatar

An Avatar object is a user photo.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>attachedObjectCode</b>
            </p>
             <p>Added</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li>
            <p><b>attachedObjectCode</b>
            </p>
             <p>Added</p>
           </li>
          </li>
        </ul>
      </td>
   <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li>
            <p><b>COPY</b>
            </p>
             <p>Added</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

### Baseline (BLIN)

Baselines are snapshots of what the performance of a project looked like at a given moment in time. They store key pieces of information about the project, like key dates, progress, cost and revenue values. 

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p>The following fields added the flag <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>budget</li>
              <li>eac</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost</li>
              <li>plannedNonBillableExpenseCost</li>
            </ul>
          </li>
          <li>
          <p>The following fields changed their type from <code>double</code> to <code>class java.math.BigDecimal</code>:
          <ul>
          <li>actualCost</li>
          <li>plannedCost</li>
          </ul>
          </li>
          <li><p><b>eac</b></p> <p>Added the flag <code>CURRENCY</code></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### BaselineTask (BSTSK)

Baselines are snapshots of what the performance of a project looked like at a given moment in time. They store key pieces of information about the project, like key dates, progress, cost and revenue values. When you create a baseline, the task information is also captured on the baseline tasks of that baseline.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p>The following fields added the flag <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost</li>
              <li>plannedNonBillableExpenseCost</li>
            </ul>
          </li>
          <li>
          <p>The following fields changed their type from <code>double</code> to <code>class java.math.BigDecimal</code>:
          <ul>
          <li>actualCost</li>
          <li>plannedCost</li>
          </ul>
          </li>
          <li><p><b>eac</b></p> <p>Added the flag <code>CURRENCY</code></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### BillingRecord (BILL)

A BillingRecord object records the revenue, hours, or expenses that can be billed. This information can be used to create invoices in an external accounting system.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p>The following fields added the flag <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>amount</li>
              <li>otherAmount</li>
            </ul>
          </li>
          <li><p><b>entryDate</b></p> <p>Added</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Category (CTGY)

A Category object is a custom form.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b>
            </p>
             <p>Added the following possible values:</p>
             <ul>
              <li><p><code>BOOKNG</code> (Booking)</p> </li>
              <li><p><code>STAFFP</code> (Staffing Plan)</p> </li>
              <li><p><code>STAFFR</code> (Staffing plan resources)</p> </li>
            </ul>
          </li>
          <li>
            <p><b>objTypes</b>
            </p>
             <p>Added the following possible values:</p>
             <ul>
              <li><p><code>BOOKNG</code> (Booking)</p> </li>
              <li><p><code>STAFFP</code> (Staffing Plan)</p> </li>
              <li><p><code>STAFFR</code> (Staffing plan resources)</p> </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### CategoryParameter (CTGYPA)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>configurations</b>
            </p>
             <p>Added</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Company (CMPY)

A Company object represents an organization consisting of a collection of people.

The Company object added the flag `SHARABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li>
            <p><b>billingRates</b>
            </p>
             <p>Added</p>
          </li>
          <li>
            <p><b>costRates</b>
            </p>
             <p>Added</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>



### CustomerPreferences (CUSTPR)

A CustomerPreferences object represents the set of preferences that a customer has set for their instance of Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>name</b>
            </p>
             <p>Added the following possible values:</p>
             <ul>
              <li><p><code>project.mgmt:default.project.singleassignmentschedule</code> (singleassignmentschedule)</p></li>
              <li><p><code>project.mgmt:logged.taskissue.move</code> (config.loggedtaskissuemove)</p></li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### ExchangeRate (EXRATE)

An ExchangeRate object represents a currency exchange rate set up in Workfront. ExchangeRate objects are not dynamic.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
           <p>The following fields changed their type from <code>double</code> to <code>class java.math.BigDecimal</code>:
          <ul>
          <li>rate</li>
      </td>
    </tr>
  </tbody>
</table>


### FinancialData (FINDAT)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p>The following fields added the flag <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualExpenseCost</li>
              <li>actualFixedRevenue</li>
              <li>actualLaborCost</li>
              <li>actualLaborCostHours</li>
              <li>actualLaborRevenue</li>
              <li>actualNonBillableExpenseCost</li>
              <li>fixedCost</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedExpenseCost</li>
              <li>plannedFixedRevenue</li>
              <li>plannedLaborCost</li>
              <li>plannedLaborCostHours</li>
              <li>plannedLaborRevenue</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>totalActualCost</li>
              <li>totalActualRevenue</li>
              <li>totalPlannedCost</li>
              <li>totalPlannedRevenue</li>
              <li>totalVarianceCost</li>
              <li>totalVarianceRevenue</li>
              <li>varianceExpenseCost</li>
              <li>varianceLaborCost</li>
              <li>varianceLaborCostHours</li>
              <li>varianceLaborRevenue</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

### Group (GROUP)

A Group object represents a set of users and teams. Groups often represent departmental structure.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>currency</b>
            </p>
             <p>Added</p>
          </li>
         </ul>
      </td>
    </tr>
  </tbody>
</table>

### Hour (HOUR)

An Hour object represents an hour logged by a user on a timesheet.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p>The following fields added the flag <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualCost</li>
              <li>resourceRevenue</li>
            </ul>
          </li>
          <li>
          <p>The following fields changed their type from <code>double</code> to <code>class java.math.BigDecimal</code>:
          <ul>
              <li>actualCost</li>
              <li>resourceRevenue</li>
          </ul>
          </li>
          <li><p><b>ratesOrigin</b></p> <p>Added</p></li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>



### OpTask (OPTASK)

An OpTask object is commonly known as an Issue. An issue is a work item that usually indicates that there is a problem preventing the completion of a task or project. An Issue can also be a Help Desk request. Change Orders, Requests, and Bugs are also Issues.

The OpTask object added the flag DOMAIN_EXTENDABLE

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p>The following fields added the flag <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualCost</li>
            </ul>
          </li>
          <li>
          <p>The following fields changed their type from <code>double</code> to <code>class java.math.BigDecimal</code>:
          <ul>
              <li>actualCost</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

### Parameter (PARAM)

A Parameter object is a custom field.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>displayType</b>
            </p>
            <p>Added the following possible values:</p>
             <ul>
              <li>
                <p><code>INTRNL</code> (Internal Lookup)</p>
              </li>
              <li>
                <p><code>MULTINTRNL</code> (Multi-Select Internal Lookup)</p>
              </li>
              <li>
                <p><code>UIEXTNSION</code> (enum.parameterdisplaytypeenum.uiextension)</p>
              </li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>



### Portfolio (PORT)

A Portfolio object is a collection of projects that compete for the same resources, typically money or people to complete them.

The Portfolio object added the flag `DOMAIN_EXTENDABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p>The following fields added the flag <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>aligned</li>
              <li>budget</li>
              <li>currency</li>
              <li>netValue</li>
              <li>onBudget</li>
              <li>onTime</li>
              <li>portfolioNetValue</li>
              <li>portfolioRoi</li>
              <li>roi</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

### Program (PRGM)

A Program object is a subset of projects within a portfolio, where similar projects can be grouped together.

The Program object added the flag `DOMAIN_EXTENDABLE`.

### Project (PROJ)

Projects are work items within Workfront, and are a main building block in the way Workfront helps people to do work. A Project object represents a group of tasks with a common, specific goal.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p>The following fields added the flag <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualBenefit</li>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualExpenseCost</li>
              <li>actualLaborCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>actualRiskCost</li>
              <li>actualValue</li>
              <li>bcwp</li>
              <li>bcws</li>
              <li>billedRevenue</li>
              <li>budget</li>
              <li>budgetedCost</li>
              <li>budgetedHours</li>
              <li>budgetedLaborCost</li>
              <li>eac</li>
              <li>fixedCost</li>
              <li>fixedRevenue</li>
              <li>plannedBenefit</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost</li>
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedRevenue</li>
              <li>plannedRiskCost</li>
              <li>plannedValue</li>
              <li>remainingCost</li>
              <li>remainingRevenue</li>
              <li>remainingRiskCost</li>
              <li>resourcePlannerBudgetedHours</li>
              <li>resourcePlannerBudgetedLaborCost</li>
              <li>riskPerformanceIndex</li>
            </ul>
          </li>
          <li>
          <p>The following fields changed their type from <code>double</code> to <code>class java.math.BigDecimal</code>:
          <ul>
          <li>actualCost</li>
          <li>actualRevenue</li>
          <li>plannedCost</li>
          <li>plannedRevenue</li>
          </ul>
          </li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>Added the flag <code>CURRENCY</code></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef (QUED)

A QueueDef object represents a Queue, which is a project that has been published to the Help Desk area to allow users to submit issues to it.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>requestorCoreAction</b>
            </p>
            <p>Added the following possible values:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Remove from Custom Data)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Add sub-projects)</p>
              </li>
              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>
            </ul>
            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>Added the following possible values:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Remove from Custom Data)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Add sub-projects)</p>
              </li>
              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>
            </ul>
            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Rate (RATE)

A Rate object represents a billing rate in Workfront.

The Rate object added the flag `ATTRIBUTE_ATTACHABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p>The following fields added the flag <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>costPerHour</li>
              <li>localBillingPerHour</li>
              <li>localCostPerHour</li>
              <li>localCurrency</li>
              <li>rateValue</li>
            </ul>
          </li>
          <li>
          <p>The following fields changed their type from <code>double</code> to <code>class java.math.BigDecimal</code>:
          <ul>
          <li>costPerHour</li>
          <li>localBillingPerHour</li>
          <li>localCostPerHour</li>
          <li>rateValue</li>
          </ul>
          </li>
         <li>
          <p>The following fields were added:
          <ul>
          <li>currency</li>
          <li>locked</li>
          <li>type</li>
          <li>value</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>
    
### Role (ROLE)

A Role object (job role) represents a functional capacity or a skill set a user might fill, such as Designer or Product Manager.

The Role object added the flag `DOMAIN_EXTENDABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p>The following fields added the flag <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>billingPerHour</li>
              <li>costPerHour</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li>
          <p>The following fields were added:
          <ul>
          <li>billingRates</li>
          <li>costRates</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScheduledReport (SCHREP)

A ScheduledReport object represents a report that has been configured to be scheduled for delivery.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>format</b>
            </p>
             <p>Added the following possible values:</p>
             <ul>
              <li>
                <p><code>tiff</code> (enum.fileextension.tiff)</p>
              </li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

A ScoreCardQuestion object represents a question that has been added to a Scorecard. These questions are usually determined by the Portfolio manager, and their answers allow the manager to understand how well a project aligns with the goals of the portfolio.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>displayType</b>
            </p>
             <p>Added the following possible values:</p>
             <ul>
              <li><p><code>INTRNL</code> (Internal Lookup)</p></li>
              <li><p><code>MULTINTRNL</code> (Multi-Select Internal Lookup)</p></li>
              <li><p><code>UIEXTNSION</code> (enum.parameterdisplaytypeenum.uiextension)</p></li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Task (TASK)

A Task object represents a work item that must be performed as a step toward achieving a final goal (completing a Project).

The Task object added the flag `DOMAIN_EXTENDABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p>The following fields added the flag <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualExpenseCost</li>
              <li>actualLaborCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost/li>
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedRevenue</li>
            </ul>
          </li>
          <li>
          <p>The following fields changed their type from <code>double</code> to <code>class java.math.BigDecimal</code>:
          <ul>
          <li>actualCost</li>
          <li>actualRevenue</li>
          <li>plannedCost</li>
          </ul>
          </li>
          <li><p><b>costType</b></p> <p>Added the following possible values:<ul><li><code>URH</code> (User and Role Hourly)</li></ul></li>
          <li><p><b>revenueType</b></p> <p>Added the following possible values:<ul><li><code>URH</code> (User and Role Hourly)</li><li><code>URC</code> (User and Role Hourly w/Cap)</li><li><code>URF</code> (User and Role Hourly Plus Fixed)</li></ul></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

costType<note>changes to possibleValues</note>
revenueType<note>changes to possibleValues</note>    


### Template (TMPL)

A Template object represents a pattern for a project. Projects can be created from templates to save time. A template contains a team and tasks, which will be copied to any project created from the template.



### TemplateTask (TTSK)

A TemplateTask object represents a Task that is part of a Template. Template Tasks become Tasks in the Project where the Template is used.



### Timesheet (TSHET)

A Timesheet object represents a virtual timecard that allows Users to enter actual hours worked for Tasks, Projects, and overhead Hour Types.



### Update (UPDATE)

Work Items in Workfront can be updated to keep users informed of the current status. An Update object represents one of these updates. Updates can be entered by users or created by the Workfront system.



### User (USER)

A User object represents a person with an account in Workfront that can log in and interact with the system.



### Work (WORK)

A Work object is a common interface that both Task and OpTask inherit, and shares common code between the two.



