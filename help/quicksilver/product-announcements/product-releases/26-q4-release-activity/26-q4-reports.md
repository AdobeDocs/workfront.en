---
title: Fourth Quarter 2026 Reporting enhancements
description: Fourth Quarter 2026 Reporting enhancements
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
---
# Fourth Quarter 2026 Reporting enhancements

This page describes Reporting enhancements made with the Fourth Quarter 2026 release to the Preview environment. These enhancements will be made available in the Production environment as noted.

For a list of all changes available at this point in the Fourth Quarter 2026 release cycle, see [Fourth Quarter 2026 release overview](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

## Enforcing end dates for scheduled reports

>[!NOTE]
>
>Preview: August 13, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

Scheduled reports now require an end date to prevent indefinite delivery. Schedules that pass their end date are automatically deactivated.

Existing schedules have been updated with end dates to improve reliability and reduce unnecessary system usage. Workfront also provides added visibility and warnings to help you manage report schedule lifecycles as they approach their end date.

For more information, see [Schedule an automatic report delivery](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

## Updated column headers for dependent connected record fields

>[!NOTE]
>
>Preview: August 13, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

We've made visual improvements to the column headers for a dependent connected record field in the table view.

For information, see [Manage dependent connections](/help/quicksilver/planning/architecture/manage-dependent-connections.md).

## Native reference fields are available for lists and reports

>[!NOTE]
>
>Preview: July 30, 2026
>Production fast release: August 13, 2026
>Production for everyone: October 15, 2026

You can now add native reference fields to lists and reports in Workfront.

A native reference field is a custom field. When the field is on a custom form attached to an object, the field is populated from the object data. For example, if the field references the Description field and it is on a custom form attached to a project, it pulls in the project description. (The field may show "N/A" if no data is available.)

For information about creating native reference fields, including the list of supported native fields, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
For information about adding fields to reports, see [Create a custom report](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Consistent ordering for multi-select field values in legacy lists and reports

>[!NOTE]
>
>Preview: July 30, 2026
>Production fast release: August 13, 2026
>Production for everyone: October 15, 2026

You now see selected options for multi-select custom fields in a consistent, predictable order on legacy lists and reports. Field order is determined by how the fields are arranged in the custom form.

![Custom form field order matches the order of selected values in a list or report](assets/new-field-order-multi-select.png)

Previously, selected options displayed in the order you chose them, or in an inconsistent order, which made rows harder to scan and compare.

Note: The new sort does not apply if the field is using text mode.
