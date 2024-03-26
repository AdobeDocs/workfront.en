---
content-type: api
navigation-topic: api-navigation-topic
title: What's new in API version 18
description: Adobe Workfront released API version 18 on April 6, 2022. API version 18 features the following changes from version 15.
author: Becky
feature: Workfront API
role: Developer
exl-id: a3d8534b-fe6e-4782-baab-7c94555ea40c
---
# What's new in API version 18

Adobe Workfront released API version 18 on <!--Date-->. API version 18 features the following changes from version 15.

## Added resources

No resources were added for API version 18.

## Removed resources

No resources were removed for API version 18

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
                <p><code>VIEW_COST_RATES</code> (View Cost Rates)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (View Billing Rates)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (View general finance)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Edit Cost Rates)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Edit Billing Rates)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Edit General Finance)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (View Cost Rates)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (View Billing Rates)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (View general finance)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Edit Cost Rates)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Edit Billing Rates)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Edit General Finance)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (View Cost Rates)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (View Billing Rates)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (View general finance)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Edit Cost Rates)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Edit Billing Rates)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Edit General Finance)</p>
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
                <p><code>VIEW_COST_RATES</code> (View Cost Rates)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (View Billing Rates)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (View general finance)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Edit Cost Rates)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Edit Billing Rates)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Edit General Finance)</p>
              </li>
            </ul>
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
                <p><code>VIEW_COST_RATES</code> (View Cost Rates)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (View Billing Rates)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (View general finance)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Edit Cost Rates)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Edit Billing Rates)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Edit General Finance)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (View Cost Rates)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (View Billing Rates)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (View general finance)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Edit Cost Rates)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Edit Billing Rates)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Edit General Finance)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (View Cost Rates)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (View Billing Rates)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (View general finance)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Edit Cost Rates)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Edit Billing Rates)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Edit General Finance)</p>
              </li>
            </ul>
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
            <p>Added the following fields:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AwaitingApproval (AWAPVL)

<table>
  <tbody>
    <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li>
            <p>Added the following operations:
            </p>
            <ul>
              <li>
                <p><b>ADD</b>
                </p>
              </li>
              <li>
                <p><b>DELETE</b>
                </p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
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
            <p>Added the following fields:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
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
            <p>Added the following fields:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
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
            <p><b>catObjCode</b>:
            </p>
            <p>Added the following possible values:
            <ul>
              <li>
                <p><code>NLBRCY</code> (Non-Labor Resource Category)
                </p>
              </li>
              <li>
                <p><code>HOUR</code> (Hour)
                </p>
              </li>
              <li>
                <p><code>RTCRD</code> (Rate card)
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>objTypes</b>:
            </p>
            <p>Added the following possible values:
            <ul>
              <li>
                <p><code>NLBRCY</code> (Non-Labor Resource Category)
                </p>
              </li>
              <li>
                <p><code>HOUR</code> (Hour)
                </p>
              </li>
              <li>
                <p><code>RTCRD</code> (Rate card)
                </p>
              </li>
             </ul>
             </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Document (DOCU)

A Document object represents a file (such as written material, images, or other forms of information).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <ul>
          <li>
            <p><b>createLargeDocument</b>:
            </p>
            <p>Added the following parameter:
            <ul>
              <li>
                <p><code>documentID</code> 
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>moveToFolder</b>:
            </p>
            <p>Added. This new action takes the following parameters:
            <ul>
              <li>
                <p><code>documentIDs</code>
                </p>
              </li>
              <li>
                <p><code>folderID</code> 
                </p>
              </li>
              <li>
                <p><code>moveToFolder</code> 
                </p>
              </li>
             </ul>
             </p>
          </li>
        </ul>
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
            <p>Added the following fields:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Default fields</td>
      <td>
        <ul>
          <li>
            <p>Added the following fields:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### JournalEntry (JRNLE)

The JournalEntry object can be set up to log information about specific object fields any time those fields are modified. When a field is set up to be logged as a part of the Journal Entry object, a corresponding Journal Entry will be created every time that field is modified.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>AAO</code> (enum.actiontypeenum.assetapproval.opened)</p>
              </li>
              <li>
                <p><code>ADM</code> (enum.actiontypeenum.assetapproval.locked.all.decisions.made)</p>
              </li>
              <li>
                <p><code>AUL</code> (enum.actiontypeenum.assetapproval.unlocked.manual)</p>
              </li>
              <li>
                <p><code>ALM</code> (enum.actiontypeenum.assetapproval.locked.manual)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### OpTask (OPTASK)

An OpTask object is commonly known as an Issue. An issue is a work item that usually indicates that there is a problem preventing the completion of a task or project. An Issue can also be a Help Desk request. Change Orders, Requests, and Bugs are also Issues.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <ul>
          <li>
            <p><b>convertToProject</b>:
            </p>
            <p>Added the following fields:
            <ul>
              <li>
                <code>copyCategories</code></li><li><code>copyNativeFields</code>
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>convertToTask</b>:
            </p>
            <p>Added the following fields:
            <ul>
              <li>
                <code>copyCategories</code></li><li><code>copyNativeFields</code>
                </p>
              </li>
             </ul>
             </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Project (PROJ)

Projects are work items within Workfront, and are a main building block in the way Workfront helps people to do work. A Project object represents a group of tasks with a common, specific goal.

### ProjectUserRole (PTEAM)

### QueueDef (QUED)

A QueueDef object represents a Queue, which is a project that has been published to the Help Desk area to allow users to submit issues to it.

### Rate (RATE)

A Rate object represents a billing rate in Workfront.

### Task (TASK)

A Task object represents a work item that must be performed as a step toward achieving a final goal (completing a Project).

### Template (TMPL)

A Template object represents a pattern for a project. Projects can be created from templates to save time. A template contains a team and tasks, which will be copied to any project created from the template.

### TemplateTask (TTSK)

A TemplateTask object represents a Task that is part of a Template. Template Tasks become Tasks in the Project where the Template is used.

### TemplateUserRole (TTEAM)

### Timesheet (TSHET)

A Timesheet object represents a virtual timecard that allows Users to enter actual hours worked for Tasks, Projects, and overhead Hour Types.

### Update (UPDATE)

Work Items in Workfront can be updated to keep users informed of the current status. An Update object represents one of these updates. Updates can be entered by users or created by the Workfront system.

### UserPrefValue (USERPF)

A UserPrefValue object represent a user preference.

### Work (WORK)

A Work object is a common interface that both Task and OpTask inherit, and shares common code between the two.
