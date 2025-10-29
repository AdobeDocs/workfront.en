---
content-type: api
navigation-topic: api-navigation-topic
title: What's new in API version 21
description: Adobe Workfront released API version 21 on October 23, 2025. API version 21 features the following changes from version 20.
author: Becky
feature: Workfront API
role: Developer
---
# What's new in API version 20

Adobe Workfront released API version 21 on October 23, 2025. API version 21 features the following changes from version 20.

## Added resources

### OriginalRequest (ORGREQ)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>entryDate</li>
          <li>ID</li>
          <li>requestID</li>
          <li>requestName</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li>ID</li>
          <li>objCode</li>
        </ul>
      </td>
 </tbody>
</table>

<!--

### StaffingPlanTemplate (SPTMPL)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
          <li>objCode</li>
        </ul>
      </td>
   <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li>ADD</li>
          <li>COUNT</li>
          <li>DELETE</li>
          <li>EDIT</li>
          <li>GET</li>
          <li>REPORT</li>
          <li>SEARCH</li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

-->

## Removed resources

### AssignmentBillingRole (ASBLRL)

The AssignmentBillingRole object and all of its fields have been removed.

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
            <p>Added the following possible value:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Edit Contact Info)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Added the following possible value:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Edit Contact Info)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Added the following possible value:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Edit Contact Info)</p>
              </li>
            </ul>
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
            <p>Added the following possible value:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Edit Contact Info)</p>
              </li>
            </ul>
         </li>
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
            <p>Added the following possible value:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Edit Contact Info)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Added the following possible value:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Edit Contact Info)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Added the following possible value:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Edit Contact Info)</p>
              </li>
            </ul>
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
              <li><p><code>AI</code></p></li>
              <li><p><code>PSD</code></p></li>
              <li><p><code>ASE</code></p></li>
              <li><p><code>INDD</code></p></li>
              <li><p><code>PUB</code></p></li>
              <li><p><code>BMP</code></p></li>
              <li><p><code>DNG</code></p></li>
              <li><p><code>HEIC</code></p></li>
              <li><p><code>HEIF</code></p></li>
              <li><p><code>JP2</code></p></li>
              <li><p><code>PJPEG</code></p></li>
              <li><p><code>RAW</code></p></li>
              <li><p><code>SVG</code></p></li>
              <li><p><code>WEBP</code></p></li>
              <li><p><code>EPS</code></p></li>
              <li><p><code>MP4</code></p></li>
              <li><p><code>MPEG</code></p></li>
              <li><p><code>WMV</code></p></li>
            </ul>
         </li>
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
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>Added</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li>
            <p><b>teamAssignments</b>
            </p>
            <p>Added</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>

### Assignment (ASSGN)

An Assignment object represents the connection between a work item and the user, team, or group that is assigned to work on it.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li>
            <p><b>assignmentBillingRoles</b>
            </p>
            <p>Removed</p>
              </li>
            </ul>
         </li>
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
              <li>
                <p><code>SPTMPL</code> (enum.categorytypeenum.staffingplantemplate)</p>
              </li>
              <li>
                <p><code>TEAMOB</code> (Team)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>objTypes</b>
            </p>
            <p>Added the following possible values:</p>
             <ul>
              <li>
                <p><code>SPTMPL</code> (enum.categorytypeenum.staffingplantemplate)</p>
              </li>
              <li>
                <p><code>TEAMOB</code> (Team)</p>
              </li>
            </ul>
          </li>
           </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Customer (CUST)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><code>APDISAB</code> (Disable use of a Java applet for timeline calculations)
            </p>
            <p>Added</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### Document (DOCU)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <ul>
          <li>
            <p><b>getTemporaryCloudURL</b>
            </p>
            <p>Added</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### DocumentFolder

The DocumentFolder object added the flag `RESTORABLE`.

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
            <p><b>getTerejectionCommentmporaryCloudURL</b>
            </p>
            <p>Added the validator <code>MAX_LENGTH</code></p>
              </li>
            </ul>
         </li>
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
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>Added</p>
              </li>
            </ul>
         </li>
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
            <p><b>dataType</b>
            </p>
            <p>Added the following possible value:</p>
             <ul>
              <li>
                <p><code>RICHLX</code> (Lexical Rich Text)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>displayType</b>
            </p>
            <p>Added the following possible value:</p>
             <ul>
              <li>
                <p><code>SNGLROLLUP</code> (Single Line Rollup)</p>
              </li></ul>
         <li>
            <p><b>isActive</b>
            </p>
            <p>Added</p>
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
            <p><b>isActive</b>
            </p>
            <p>Added</p>
           </li>
           </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Portfolio (PORT)

A Portfolio object is a collection of projects that compete for the same resources, typically money or people to complete them.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>overrideCurrency</b>
            </p>
            <p>Added</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### Program (PRGM)

A Program object is a subset of projects within a portfolio, where similar projects can be grouped together.

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
         </li>
      </td>
    </tr>
  </tbody>
</table>

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
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>Added</p>
              </li>
            </ul>
         </li>
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
            <p>Added the following possible value:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Edit Contact Info)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>Added the following possible value:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Edit Contact Info)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <ul>
          <li>
            <p><b>helpDeskProjects</b>
            </p>
            <p>Added</p>
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

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>localBillingPerHour</b>
            </p>
            <p>Removed</p>
              </li>
          <li>
            <p><b>localCostPerHour</b>
            </p>
            <p>Removed</p>
              </li>
         </li>
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
              <li><p><code>AI</code></p></li>
              <li><p><code>PSD</code></p></li>
              <li><p><code>ASE</code></p></li>
              <li><p><code>INDD</code></p></li>
              <li><p><code>PUB</code></p></li>
              <li><p><code>BMP</code></p></li>
              <li><p><code>DNG</code></p></li>
              <li><p><code>HEIC</code></p></li>
              <li><p><code>HEIF</code></p></li>
              <li><p><code>JP2</code></p></li>
              <li><p><code>PJPEG</code></p></li>
              <li><p><code>RAW</code></p></li>
              <li><p><code>SVG</code></p></li>
              <li><p><code>WEBP</code></p></li>
              <li><p><code>EPS</code></p></li>
              <li><p><code>MP4</code></p></li>
              <li><p><code>FLV</code></p></li>
              <li><p><code>M4V</code></p></li>
              <li><p><code>MPEG</code></p></li>
              <li><p><code>WMV</code></p></li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

A ScoreCardQuestion object represents a question that has been added to a Scorecard. These questions are usually determined by the Portfolio manager, and their answers allow the manager to understand how well a project aligns with the goals of the portfolio.<table>
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
            <p>Added the following possible value:</p>
             <ul>
              <li>
                <p><code>SNGLROLLUP</code> (Single Line Rollup)</p>
              </li></ul>
         </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### StaffingPlan

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>totalEstimatedCost</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedHours</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedRevenue</b>
            </p>
            <p>Added</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

-->

<!--

### StaffingPlanResource

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>totalEstimatedCost</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedHours</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedRevenue</b>
            </p>
            <p>Added</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

-->

### Task (TASK)

A Task object represents a work item that must be performed as a step toward achieving a final goal (completing a Project).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>Added</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li>
            <p><b>teamAssignments</b>
            </p>
            <p>Added</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>

### Team

The Team object added the flags `DATA_EXTENDIBLE` and `SHARABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>categoryID</b>
            </p>
            <p>Added</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li>
            <p><b>category</b>
            </p>
            <p>Added</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li>
            <p><b>objectCategories</b>
            </p>
            <p>Added</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>


### TemplateAssignment

The TemplateAssignment object added the flag `ATTRIBUTE_ATTACHABLE`.

### Timesheet (TSHET)

A Timesheet object represents a virtual timecard that allows Users to enter actual hours worked for Tasks, Projects, and overhead Hour Types.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Core fields</td>
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

### Work (WORK)

A Work object is a common interface that both Task and OpTask inherit, and shares common code between the two.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>Added</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li>
            <p><b>teamAssignments</b>
            </p>
            <p>Added</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>


