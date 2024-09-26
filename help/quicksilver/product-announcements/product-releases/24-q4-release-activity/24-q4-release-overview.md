---
title: Fourth Quarter 2024 release overview
description: This page provides information about functionality that is included in the Fourth Quarter 2024 release. These enhancements are planned to become available in the Production environment throughout the quarter.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6cc67488-1ba9-4455-9152-366aaabf0939
---
# Fourth Quarter 2024 release overview

This page provides information about functionality that is included in the Fourth Quarter 2024 release. These enhancements are planned to become available in the Production environment throughout the quarter.

<span class="preview">Off-cycle features (those releasing to Production prior to the Fourth Quarter 2024 release date) are highlighted in yellow.</span>

>[!IMPORTANT]
>
>The 23.3 release included the option to move your organization to monthly releases. Therefore, Workfront has changed the numbering scheme of releases to account for both monthly and quarterly release tracks. The first number designates the year, and the second number signifies the month of the release. Example: The release for April, 2024 reads as 24.4.
>
>Monthly and quarterly releases are planned to be available on the Thursday of the second full week of the month, unless otherwise specified.
>
>|Monthly release|Quarterly release|
>|----|----|
>|<ul><li>24.8 (August 15, 2024)</li><li>24.9 (September 12, 2024)</li><li>24.10 (October 2024)</li></ul>| <ul><li>24.10 (October 2024)</li></ul>|
>
>Note that for the final release of each quarter (24.10 this quarter), users on the fast release schedule will receive the release one day early.
>
>For more information on the fast release process, see [Enable or disable the fast release process](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Adobe Workfront enhancements

* [Administrator enhancements](#administrator-enhancements)
* [Integration enhancements](#integration-enhancements)
* [Project enhancements](#project-enhancements)
* [Proofing enhancements](#proofing-enhancements)
* [Report and Dashboard enhancements](#report-and-dashboard-enhancements)
* [Other enhancements](#other-enhancements)
* [Functionality soon to be removed from Workfront](#functionality-soon-to-be-removed-from-workfront)

### Administrator enhancements

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Feature</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Release dates</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">A "Select all" option is now available in layout templates</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>To help you more easily display and hide fields with layout templates, a "Select all" check box was added to the Overview and Finance areas of the Details view in a layout template. This option is available when you have selected Project, Task, Issue, Portfolio, or Program under under "Customize what users see".</p>
                    </td>
                    <td><p><b>Available on these dates:</b></p>
                        <ul>
                            <li>
                                <p>Preview release: August 29, 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Production release for all customers: August 29, 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Roll back environment promotion packages</a></p>
                        [!BADGE In production for Fast Release ]{type=Positive}
                        <p>To make environment promotion more flexible and easier to use, we've enabled rollback functionality. Now, you can roll back packages within 24 hours, allowing you to more easily restore previous configurations that have been affected by an environment promotion package.</p>
                    </td>
                    <td><p><b>Available on these dates:</b></p>
                        <ul>
                            <li>
                                <p>Preview release: August 29, 2024</p>
                            </li>
                            <li>
                                <p>Production for fast release: With the 24.9 release (September 12, 2024)</p>
                            </li>
                            <li>
                                <p>Production release for all customers: With the 24.10 release (October 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Layout button on the custom form designer allows two or three columns</a></p>
                        <p>A "Layout" button on the custom form designer allows you to choose from a two- or three-column working area. The original form designer uses three columns and the field settings are displayed in the far right column. If you select two columns, the field settings are displayed next to the field library in the far left column.</p>
                    </td>
                    <td><p><b>Available on these dates:</b></p>
                        <ul>
                            <li>
                                <p><s>Preview release: August 12, 2024</s></p>
                            </li>
                            <li>
                                <p>Production for fast release: N/A</p>
                            </li>
                            <li>
                                <p>Production release for all customers: N/A</p>
                            </li>
                        </ul>
                        <p><i>This feature has been removed from Preview and will not be released with any future releases.</i></p>
                    </td>
                </tr>
           </tbody>
        </table>

### Integration enhancements

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Feature</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Release dates</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Outlook integration login experience enhancements</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>The login experience for Outlook integration has been streamlined so that all customers see the same button to log in to Workfront whether or not they are IMS-enabled. The subsequent login steps remain different for IMS and non-IMS instances, but the initial page is the same for all users.</p>
                    </td>
                    <td><p><b>Available on these dates:</b></p>
                        <ul>
                            <li>
                                <p>Preview release: August 6, 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Production release for all customers: August 6, 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### Project enhancements

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Feature</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Release dates</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">More relevant assignments added to the New Task workflow</a></p>
                        [!BADGE In production for Fast Release ]{type=Positive}
                        <p>We have added the same functionality for more relevant smart assignments to the Assignments field in the New Task box when adding a task to a project and in a project task list.</p>
                    </td>
                    <td><p><b>Available on these dates:</b></p>
                        <ul>
                            <li>
                                <p>Preview release: February 13, 2024</p>
                            </li>
                            <li>
                                <p>Production for fast release: With the 24.5 release (May 16, 2024)</p>
                            </li>
                            <li>
                                <p>Production release for all customers: With the 24.10 release (October 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">More relevant smart assignments</a></p>
                        [!BADGE In production for Fast Release ]{type=Positive}
                        <p>We have changed the algorithm that Workfront uses to calculate and suggest smart assignments for tasks. The new algorithm applies in the following areas in Workfront where you assign a task: task lists, the Assignments area in the task header, Home, and the Summary panel.</p>
                    </td>
                    <td><p><b>Available on these dates:</b></p>
                        <ul>
                            <li>
                                <p>Preview release: December 21, 2023</p>
                            </li>
                            <li>
                                <p>Production for fast release: With the 24.5 release (May 16, 2024)</p>
                            </li>
                            <li>
                                <p>Production release for all customers: With the 24.10 release (October 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### Proofing enhancements

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Feature</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Release dates</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Blank screen fix for Desktop Proofing Viewer Windows users</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>We fixed an issue with the new 2.1.36 Desktop Proofing Viewer version which caused some Windows users to see a blank screen after opening the viewer. </p>
                        <p>New version for Windows users: 2.1.37</p>
                    </td>
                    <td><p><b>Available on these dates:</b></p>
                        <ul>
                            <li>
                                <p>Preview release: August 30, 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Production release for all customers: August 30, 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Chromium update for the Desktop Proofing Viewer</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>We are upgrading the Desktop Proofing Viewer to support Chromium 126.0.6478.127 which will resolve issues with UI elements in interactive proofs.</p>
                    </td>
                    <td><p><b>Available on these dates:</b></p>
                        <ul>
                            <li>
                                <p>Preview release: August 29, 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Production release for all customers: August 29, 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>        

### Report and Dashboard enhancements

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Feature</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Release dates</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-report-and-dashboard-enhancements.md" class="MCXref xref" xrefformat="{para}">Workfront Data Connect available for new plans</a></p>
                        <p>Workfront Data Connect will become available for organizations on one of the new Workfront plans. Data Connect allows organizations to access their data as a secure and scalable data lake, which can be analyzed and visualized using business intelligence tools or stored externally. Additionally, organizations can use Data Connect to view data analytics that were previously unavailable, such as time-based trend analysis, variable mapping, and analysis of external system data in combination with Workfront data.</p>
                    </td>
                    <td><p><b>Available on these dates:</b></p>
                        <ul>
                            <li>
                                <p><span class="preview">Production release for all customers: With the 24.10 release (October 2024)</span></p>
                            </li>
                        </ul>
                        <p><i>Only available for organizations on one of the new Adobe Workfront plans. Data Connect is included in the Ultimate plan or can be purchased as an add-on to the Prime and Select plans.</i></p>
                    </td>
                </tr>
           </tbody>
        </table>    

### Other enhancements

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-24-q4.md" class="MCXref xref" xrefformat="{para}">General availability of Adobe Workfront Planning</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Workfront Planning is available for all customers who purchased a Workfront Planning license, in addition to their Workfront license. Contact your account representative for more information about Workfront Planning.</p>
                        <p>For the latest Workfront Planning release information each quarter, see the <a href="#workfront-planning-enhancements">Workfront Planning enhancements</a> section below.</p>
                    </td>
                    <td><p><b>Available on these dates:</b></p>
                        <ul>
                            <li>
                                <p><span class="preview">Production release for all customers: August 28, 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Adobe AI Assistant available in Workfront</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>To make it easier for you to accomplish your work, we've added Adobe's AI Assistant to Workfront. AI Assistant can help you by:</p>
                        <ul>
                            <li>Summarizing work items and documents, allowing you to quickly gain a general understanding of tasks, projects, and assets.</li>
                            <li>Providing information from Experience League documentation, bringing instructions and reference material into Workfront, while linking to more in-depth documentation.</li>
                            <li>Creating and refining formulas for calculated custom form fields, generating formulas from text prompts, or locating errors in existing formulas.</li>
                            </ul>
                            <p>Your Workfront administrator can enable or disable AI Assistant for your organization. The AI Assistant is available for instances with Select, Prime, and Ultimate plans.</p>
                        </td>
                    <td><p><b>Available on these dates:</b></p>
                        <ul>
                            <li>
                                <p>Preview release: August 28, 2024</p>
                            </li>
                            <li>
                                <p class="preview">Production release: August 28, 2024</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Look-and-feel updates during the Fourth Quarter 2024 timeframe</a></p>
                        <p>Minor updates to the look and feel of various areas of the Adobe Workfront application are being made within the Fourth Quarter 2024 timeframe. Review the individual release notes for specific release dates.</p>
                    </td>
                    <td><p><b>Available on these dates:</b></p>
                        <ul>
                            <li>
                                <p>Preview release: Throughout the Fourth Quarter 2024 release timeframe</p>
                            </li>
                            <li>
                                <p><span class="preview">Production release: Review the release notes for specific dates</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                            
           </tbody>
        </table>   

### Functionality soon to be removed from Workfront

The following functionality is soon to be removed from Workfront:

#### Deprecation of the legacy Home experience with 24.10

We will be officially deprecating the legacy Home experience with the 24.10 release. Users are encouraged to begin using new Home, which will continue to be enhanced with additional features prior to the deprecation. For more information about the transition, including advice about what users and administrators can do to prepare, see [Legacy Home deprecation guide](/help/quicksilver/product-announcements/announcements/legacy-home-deprecation.md).

## Announcements

### Workfront Fusion enhancements

New features in Workfront Fusion are available in Production at a cadence outside of the Fourth Quarter 2024 release schedule. For more information about the latest features, see [Adobe Workfront Fusion release activity](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Workfront Planning enhancements

New features in Workfront Planning are available in Production. For more information about the latest features, see [Adobe Workfront Planning Fourth Quarter 2024 release activity](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-24-q4.md).

### Workfront Scenario Planner enhancements

There are no Scenario Planner updates at this point in the release. This area will be updated when updates are available.

### Workfront Proof enhancements

There are no Workfront Proof updates at this point in the release. This area will be updated when updates are available.

### Workfront Goals enhancements

There are no Workfront Goals updates at this point in the release. This area will be updated when updates are available.

### API version 18

For API version 18, we've modified some resources and endpoints. Some of the changes support new functionality, and others make it easier for you to use the information available through the API.

For information on what's new and updated, see [What's new in API version 18](/help/quicksilver/wf-api/api/new-api-version-18.md).

For information on API versions, see [API versioning and support schedule](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Workfront Maintenance Updates

For information about the maintenance updates made during the Fourth Quarter 2024 release, see [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Training updates

Explore the latest updates made to learning programs, learning paths, videos, and guides for each Adobe Workfront product release. For more information, see the "What's New" section of the [Workfront Tutorials page](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html).
