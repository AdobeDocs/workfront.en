---
content-type: api
navigation-topic: api-navigation-topic
title: What's new in API version 17
description: Adobe Workfront released API version 17 on April 6, 2022. API version 17 features the following changes from version 15.
author: Becky
feature: Workfront API
---
# What's new in API version 17

Adobe Workfront released API version 17 on October 12, 2023. API version 17 features the following changes from version 16.

## Added resources

<!--

### Booking (BOOKNG)

-->

### ExternalDocument (EXTDOC)

An ExternalDocument object is a document or other digital asset that is located in a document storage provider external to Workfront. These assets can be linked to and from Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><p><b>dateModified</b></p></li>
          <li><p><b>description</b></p></li>
          <li><p><b>documentProviderID</b></p></li>
          <li><p><b>ext</b></p></li>
          <li><p><b>fileType</b></p></li>
          <li><p><b>iconURL</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>name</b></p></li>
          <li><p><b>path</b></p></li>
          <li><p><b>providerType</b></p></li>
          <li><p><b>readOnly</b></p></li>
          <li><p><b>size</b></p></li>
          <li><p><b>thumbnailURL</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><p><b>dateModified</b></p></li>
          <li><p><b>description</b></p></li>
          <li><p><b>documentProviderID</b></p></li>
          <li><p><b>ext</b></p></li>
          <li><p><b>fileType</b></p></li>
          <li><p><b>iconURL</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>isGoogleRootItem</b></p></li>
          <li><p><b>isTeamDriveItem</b></p></li>
          <li><p><b>name</b></p></li>
          <li><p><b>objCode</b></p></li>
          <li><p><b>path</b></p></li>
          <li><p><b>providerType</b></p></li>
          <li><p><b>readOnly</b></p></li>
          <li><p><b>size</b></p></li>
          <li><p><b>thumbnailURL</b></p></li>
          <li><p><b>value</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Default fields</td>
      <td>
        <ul>
          <li><p><b>ID</b></p></li>
          <li><p><b>name</b></p></li>
          <li><p><b>objCode</b></p></li>
        </ul>
      </td>
    </tr>
    </tr>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <ul>
          <li><p><b>browseListWithLinkAction</b></p></li>
          <li><p><b>getDocumentDownloadUrl</b></p></li>
          <li><p><b>getRootFolderID</b></p></li>
          <li><p><b>getRootFolderIDFromDB</b></p></li>
          <li><p><b>linkExternalDocumentObjects</b></p></li>
          <li><p><b>setLinkedFolderMetadata</b></p></li>
        </ul>
      </td>
    </tr>
    </tr>
    <tr>
      <td role="rowheader">Queries</td>
      <td>
        <ul>
          <li><p><b>browseList</b></p></li>
          <li><p><b>getFolderMetaData</b></p></li>
          <li><p><b>searchExternalDocuments</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li><p><b>SEARCH</b></p></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### NlbrGroups (NLBRGP)

### NonLaborResource (NLBR)

### NonLaborResourceParameterValue (NLBRPV)

### RichTextNonLaborResourceParameterValue (NLRRPV)

-->

### UserLocation (USRLOC)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><p><b>classifierID</b></p></li>
          <li><p><b>customerID</b></p></li>
          <li><p><b>endDate</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>isCurrent</b></p></li>
          <li><p><b>startDate</b></p></li>
          <li><p><b>userID</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><p><b>customer</b></p></li>
          <li><p><b>user</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><p><b>ID</b></p></li>
          <li><p><b>objCode</b></p></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

## Removed resources

No resources were removed for API version 17

## Modified resources

The following resources were modified for API version 17.

<!--

### AccessLevel (ACSLVL)

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

### AccessRequest (ACSREQ)

If a User does not have access to an object in Workfront that they need, they can request access to that object. The AccessRequest object represents this request.

### AccessRule (ACSRUL)

An AccessRule object represents a rule set in custom access levels that determines how users can share projects they create.

-->

### Baseline (BLIN)

Baselines are snapshots of what the performance of a project looked like at a given moment in time. They store key pieces of information about the project, like key dates, progress, cost and revenue values. 

The Baseline object removed the flag **INLINE_EDITABLE**.

### BillingRecord (BILL)

A BillingRecord object records the revenue, hours, or expenses that can be billed. This information can be used to create invoices in an external accounting system.

The BillingRecord object removed the flag **INLINE_EDITABLE**.

<!--

### Category (CTGY)

A Category object is a custom form.

-->

### Company (CMPY)

A Company object represents an organization consisting of a collection of people.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>Removed</p>
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
            <p>Added the possible value "config.defaultToNewHomeDescription" (customer:config.defaultToNewHome)>/p?<p>This allows an organization to make the new Home experience the default for its users.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### DocumentVersion (DOCV)

A DocumentVersion object represents a specific version of a file (such as written material, images, or other forms of information).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>externalIntegrationType</b>
            </p>
            <p>Added the possible value "Frame.io" (FRAMEIO)</p>
          </li>
          <li>
            <p><b>fileType</b>
            </p>
            <p>Added the possible value "enum.filetype.site" (site)</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### ExchangeRate (EXRATE)

An ExchangeRate object represent a currency exchange rate set up in Workfront. ExchangeRate objects are not dynamic.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>The following fields were added:
        <ul>
          <li><p><b>endDate</b></p></li>
          <li><p><b>startDate</b></p></li>
       </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <ul>
          <li><p><b>getCustomerCurrencies</b></p></li>
          <p>Added.</p>
       </ul>
      </td>
    </tr>
 </tbody>
</table>

### Expense (EXPNS)

Expenses represent the non-labor costs that might be incurred during the life of a project. 

The Expense object removed the flag **INLINE_EDITABLE**.

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
            <p><b>defaultInterface</b>
            </p>
            <p>Removed</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Hour (HOUR)

An Hour object represents an hour logged by a user on a timesheet.

The Hour object removed the flag **INLINE_EDITABLE**.

### Iteration (ITRN)

An Iteration object represents a single Agile Iteration. Iterations are discrete periods of time used to plan and complete Agile stories.

The Iteration object removed the flag **INLINE_EDITABLE**.


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
              <li>Added approver (AAA)</li>
              <li>Added reviewer (AAR)</li>
              <li>Removed reviewer (ARR)</li>
              <li>Removed approver (ARA)</li>
              <li>Decision approved (ADA)</li>
              <li>Decision approved with changes (ADC)</li>
              <li>Decision needs work (ADN)</li>
              <li>Decision revoked (ADR)</li>
              <li>Approver changed (AAC)</li>
              <li>Reviewer changed (ARC)</li>
              <li>Review complete (RDC)</li>
              <li>Review revoked (RDR)</li>
              <li>Publish (PUB)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Kanban Board (KNBNBD)

A Kanban board is used to track tasks in an Agile environment.

The Kanban Board object removed the flag **INLINE_EDITABLE**.


### LinkedFolder (LNKFDR)

A LinkedFolder object represents a folder linked from an external document provider, such as Google Drive or Dropbox.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>externalIntegrationType</b>
            </p>
            <p>Added possible value "Frame.io (FRAMEIO)</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### OpTask / Issue (OPTASK)

An OpTask object is commonly known as an Issue. An issue is a work item that usually indicates that there is a problem preventing the completion of a task or project. An Issue can also be a Help Desk request. Change Orders, Requests, and Bugs are also Issues.

The Issue object removed the flag **INLINE_EDITABLE**.

### Project (PROJ)

Projects are work items within Workfront, and are a main building block in the way Workfront helps people to do work. A Project object represents a group of tasks with a common, specific goal.

The Project object removed the flag **INLINE_EDITABLE**.

### ProjectUser (PRTU)

A ProjectUser object represents a user associated with a specific project.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Added.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Added.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### QueueDef (QUED)

A QueueDef object represents a Queue, which is a project that has been published to the Help Desk area to allow users to submit issues to it.

-->

### Rate (RATE)

A Rate object represents a billing rate in Workfront.

The Rate object removed the flag **INLINE_EDITABLE**.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Actions</td>
      <td>The following actions have been added to support Rate Card functionality:
        <ul>
          <li><p><b>deleteRateForRole</b></p></li>
          <li><p><b>editRatesForRole</b></p></li>
          <li><p><b>getUsedClassifierIds</b></p></li>
          <li><p><b>setRatesFromRateCard</b></p></li>
        </ul>
        <p>The <b>setRatesForRole</b> action has been modified to add the following fields:
        <ul>
        <li>classifierID</li>
        <li>currencyCode</li>
        <li>sourceRateCardID</li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Risk (RISK)

A Risk object represents a possible event that may prevent a project from finishing on time or within budget. Risks are added to projects in the planning phase to identify potential obstacles prior to the approval of any work.

The Risk object removed the flag **INLINE_EDITABLE**.

### Role / Job Role (ROLE)

A Role object (job role) represents a functional capacity or a skill set a user might fill, such as Designer or Product Manager.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>Removed</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Task (TASK)

A Task object represents a work item that must be performed as a step toward achieving a final goal (completing a Project).

The Task object removed the flag **INLINE_EDITABLE**.

### Team (TEAMOB)

A Team object is a collection of Users that can be assigned to a work item.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>Removed</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### TeamMember (TEAMMB)

A TeamMember object is a user associated with a specific team.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Added.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Added.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### TemplateUser (TMTU)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Added.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Added.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Timesheet (TSHET)

A Timesheet object represents a virtual timecard that allows Users to enter actual hours worked for Tasks, Projects, and overhead Hour Types.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>objCode</b>
            </p>
            <p>Removed</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Update (UPDATE)

Work Items in Workfront can be updated to keep users informed of the current status. An Update object represents one of these updates. Updates can be entered by users or created by the Workfront system.

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
            <p>Added the following values:</p>
            <ul>
              <li>Added approver (assetapprovalAddApprover)</li>
              <li>Added reviewer (assetapprovalAddReviewer)</li>
              <li>Removed approver (assetapprovalRemoveApprover)</li>
              <li>Removed reviewer (assetapprovalRemoveReviewer)</li>
              <li>Decision approved (assetapprovalDecisionApproved)</li>
              <li>Decision needs work (assetapprovalDecisionNeedsWork)</li>
              <li>Decision approved with changes (assetapprovalDecisionApprovedChanges)</li>
              <li>Decision revoked (assetapprovalDecisionRevoked)</li>
              <li>Approver changed (assetapprovalApproverChanged)</li>
              <li>Reviewer changed (assetapprovalReviewerChanged)</li>
              <li>Review complete (assetapprovalReviewerDecisionComplete)</li>
              <li>Review revoked (assetapprovalReviewerDecisionRevoked)</li>
              <li>External document send error (externalDocumentSendError)</li>
              <li>Document version published (documentVersionPublish)</li>
              <li>Linked folder workflow (linkedFolderWorkflow)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
 </table>

### User (USER)

A User object represents a person with an account in Workfront that can log in and interact with the system.

The User object removed the flag **INLINE_EDITABLE**.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>workTime</b>
            </p>
            <p>This field has been added, and is a number between 0 and 1 that represents the percentage of time that a user can spend on project work (non-overhead work) each day. A value of 1 means the user can spend 100% of their time on project work.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li>
            <p><b>userLocations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### UserGroups (USRGPS)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Added.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Added.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### UserNote (USRNOT)

A UserNote object is a notification.

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
            <p>Added the following values:</p>
            <ul>
              <li>Document needs your approval (AAA)</li>
              <li>Document needs your review (AAR)</li>
              <li>Document no longer needs your approval (ARA)</li>
              <li>Document no longer needs your review (ARR)</li>
              <li>Document needs (user)'s approval (ATA)</li>
              <li>Document needs (user)'s review (ATR)</li>
              <li>Document no longer needs (user)'s approval (RTA)</li>
              <li>Document no longer needs (user)'s review (RTR)</li>
              <li>Document approved (ADA)</li>
              <li>Document approved with changes (ADC)</li>
              <li>Document needs work (ADN)</li>
              <li>(User) has marked (document) as approved. Your approval is no longer needed. (AAN)</li>
              <li>(User) has marked (document) as approved with changes. Your approval is no longer needed. (ACN)</li>
              <li>(User) has marked (document) as needs work. Your approval is no longer needed. (AWN)</li>
              <li>Document needs your review now rather than approval (AAC)</li>
              <li>Document needs your approval now rather than a review (ADN)</li>
              <li>Document reviewed (RDC)</li>
              <li>Document reviewed (TRC)</li>
              <li>(User) has reviewed (document) as complete. Your review is no longer needed. (TRN)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### UserRole (USRROL)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Added.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Added.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
