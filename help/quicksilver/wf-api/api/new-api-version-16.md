---
content-type: api
navigation-topic: api-navigation-topic
title: What's new in API version 16
description: Adobe Workfront released API version 16 on April 6, 2022. API version 16 features the following changes from version 15.
author: Becky
feature: Workfront API
exl-id: 1cfdc136-f3b4-4beb-b58b-f546a5510e6d
---
# What's new in API version 16

Adobe Workfront released API version 16 on April 6, 2022. API version 16 features the following changes from version 15.

## Added resources

No resources were added for API version 16.

## Removed resources

No resources were removed for API version 16

## Modified resources

AccessLevel (ACSLVL)
Approval (APPROVAL)
CustomerPreferences (CUSTPR)
ExternalSection (EXTSEC)
Hour (HOUR)
LayoutTemplate (LYTMPL)
Note (NOTE)
OpTask / Issue (OPTASK)
Project (PROJ)
Rate (RATE)
RichTextNote (RHNOTE)
Role / Job Role (ROLE)
Task (TASK)
UIFilter / Filter (UIFT)
UIGroupBy / Grouping (UIGB)
UIView / View (UIVW)
User (USER)
UserNote (USRNOT)

### AccessLevel (ACSLVL)

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>LicenseType</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code><!--x--></code></p>
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
            <p><b>resourcePlannerBudgetedHours</b>
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
              <li>
                <p><code>customer:config.general.autoupgradedisabled</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">actions</td>
      <td>
        <ul>
          <li>
            <p><b>getIsAutoUpgradeDisabled</b>
            </p>
            <p>This action returns a boolean that describes whether the customer has disabled the option to auto-upgrade Contributer license holders.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### ExternalSection (EXTSEC)

An ExternalSection object is an external web page that is embedded in a Workfront report.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">actions</td>
      <td>
        <ul>
           <li>
            <p><b>calculateIframeURL</b>
            </p>
            <p><!--x--></p>
         </li>
          <li>
            <p><b>calculateIframeURLS</b>
            </p>
            <p><!--x--></p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
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
            <p><b>timesheetHourIdentifier</b>
            </p>
            <p>Added. This parameter <!--x-->. </p>
           </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### LayoutTemplate (UITMPL)

Adobe Workfront administrators or group administrators can create templates to customize the layout elements in Adobe Workfront. A LayoutTemplate object represents one of these templates.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>LicenseType</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code><!--x--></code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Note (NOTE)

A Note object is a comment or update made on a Workfront object.



### OpTask / Issue (OPTASK)

An OpTask object is commonly known as an Issue. An issue is a work item that usually indicates that there is a problem preventing the completion of a task or project. An Issue can also be a Help Desk request. Change Orders, Requests, and Bugs are also Issues.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">actions</td>
      <td>
        <ul>
           <li>
            <p><b>assignMultiple</b>
            </p>
            <p>This action added the field <code>teamIDs</code> to support the functionality of assigning multiple teams to a task or issue.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Project (PROJ)

Projects are work items within Workfront, and are a main building block in the way Workfront helps people to do work. A Project object represents a group of tasks with a common, specific goal.



### Rate (RATE)

A Rate object represents a billing rate in Workfront.



### RichTextNote (RHNOTE)

A RichTextNote object is a comment or update made on a Workfront object, that includes rich text such as bold or italicized text.

The RichTextNote object removed the flag `REPORTABLE`.

### Role / Job Role (ROLE)

A Role object (job role) represents a functional capacity or a skill set a user might fill, such as Designer or Product Manager.



### Task (TASK)

A Task object represents a work item that must be performed as a step toward achieving a final goal (completing a Project).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">actions</td>
      <td>
        <ul>
           <li>
            <p><b>assignMultiple</b>
            </p>
            <p>This action added the field <code>teamIDs</code> to support the functionality of assigning multiple teams to a task or issue.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIFilter / Filter (UIFT)



<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">actions</td>
      <td>
        <ul>
          <li>
            <p><b>addJoinForNullableFields</b>
            </p>
            <p><!--x--></p>
         </li>
         <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>These actions support the ability to share filters, views, and groupings system-wide.</p><p>For more information, see <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">Make filters, views, or groupings available to all users</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIGroupBy / Grouping (UIGB)


<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">actions</td>
      <td>
        <ul>
          <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>These actions support the ability to share filters, views, and groupings system-wide.</p><p>For more information, see <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">Make filters, views, or groupings available to all users</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### UIView / View (UIVW)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>layoutType</b>
            </p>
            <p>Added the following possible value:</p>
            <ul>
              <li>
                <p><code>WLIST</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">actions</td>
      <td>
        <ul>
          <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>These actions support the ability to share filters, views, and groupings system-wide.</p><p>For more information, see <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">Make filters, views, or groupings available to all users</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>




### User (USER)

A User object represents a person with an account in Workfront that can log in and interact with the system.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>LicenseType</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code><!--x--></code></p>
              </li>
            </ul>
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
      <td role="rowheader">Queries</td>
      <td>
        <ul>
          <li>
            <p><b>myAllObjectTypesUnreadNotifications</b>
            </p>
            <p>Added the following possible value:
            <ul>
            <li>
            includeAll
            </li>
            </ul>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

