# Release Notes Reference Templates

Detailed templates for each release note page type. These are based on the templates in
`help/quicksilver/product-announcements/product-releases/release-note-templates/` and
the actual formatting used in recent quarterly releases.

---

## Product Area Page Template

```markdown
---
title: {Written Quarter} {Year} {Area} enhancements
description: {Written Quarter} {Year} {Area} enhancements
author: {Author}
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: {existing UUID}
---
# {Written Quarter} {Year} {Area} enhancements

This page describes {Area} enhancements made with the {Written Quarter} {Year} release to the Preview environment. These enhancements will be made available in the Production environment as noted.

For a list of all changes available at this point in the {Written Quarter} {Year} release cycle, see [{Written Quarter} {Year} release overview](/help/quicksilver/product-announcements/product-releases/{YY}-q{N}-release-activity/{YY}-q{N}-release-overview.md).

## Feature Title Here

>[!NOTE]
>
>Preview: {Month Day, Year}
>Production fast release: {Month Day, Year}
>Production for everyone: {Month Day, Year}

Feature description paragraph.

For more information, see [Help article title](/help/quicksilver/path/to/article.md).
```

### Rules for Product Area Pages

- Use markdown (not HTML) for body content
- Each feature gets an H2 heading
- The `>[!NOTE]` callout must have a blank line before it
- The `>[!NOTE]` format is exactly:
  ```
  >[!NOTE]
  >
  >Preview: {date}
  >Production fast release: {date}
  >Production for everyone: {date}
  ```
- If a feature was temporarily removed, add a line after the date:
  ```
  >
  >This feature has been temporarily removed from the Production environment on {date}.
  ```
- Help links use absolute paths starting with `/help/quicksilver/`

---

## Overview Page Template

```markdown
---
title: {Written Quarter} {Year} release overview
description: This page provides information about functionality that is included in the {Written Quarter} {Year} release. These enhancements are planned to become available in the Production environment throughout the quarter.
author: {Author}
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: {existing UUID}
---
# {Written Quarter} {Year} release overview

This page provides information about functionality that is included in the {Written Quarter} {Year} release scheduled for {Release Month} {Year}.

The enhancements on this page are available in the Preview environment. This page will be updated with additional enhancements as the {Written Quarter} {Year} release nears its planned Production release.

>[!IMPORTANT]
>
>
>Monthly and quarterly releases are planned to be available on the Thursday of the second full week of the month, unless otherwise specified.
>
>|Monthly release|Quarterly release|
>|----|----|
>|<ul><li>{VV}.{M} ({Month Day, Year})</li><li>{VV}.{M} ({Month Day, Year})</li><li>{VV}.{M} ({Month Day, Year})</li></ul>|<ul><li>{VV}.{M} ({Month Day, Year})</li></ul>|
>
>Note that for the final release of each quarter ({VV}.{M} this quarter), users on the fast release schedule will receive the release one day early ({Month Day, Year}).
>
>For more information on the fast release process, see [Enable or disable the fast release process](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Adobe Workfront enhancements

* [Administrator enhancements](#administrator-enhancements)
* [Document enhancements](#document-enhancements)
* [Project enhancements](#project-enhancements)
* [Reporting enhancements](#reporting-enhancements)
* [Requesting enhancements](#requesting-enhancements)
* [Other enhancements](#other-enhancements)
```

### Overview Feature Table

Each H3 product area section contains an HTML table. Use this exact structure:

```html
### {Area} enhancements

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
              <tr>
        <td><strong>Feature</strong>
        </td>
        <td><strong>Preview</strong></td>
        <td><strong>Fast release</strong></td>
        <td><strong>Quarterly</strong></td>
        </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/{YY}-q{N}-release-activity/{YY}-q{N}-{area}.md" class="MCXref xref" xrefformat="{para}">Feature Title</a><p>Short description of the feature.</p>
        </td>
        <td><p>{Month Day, Year}</p></td>
        <td><p>{Month Day, Year}</p></td>
        <td><p>{Month Day, Year}</p></td>
    </tr>
            </tbody>
        </table>
```

#### Table rules

- Feature cell: `<a>` tag with `class="MCXref xref" xrefformat="{para}"` followed by `<p>` description
- The `href` links to the product area page (not a specific anchor)
- Date cells: wrapped in `<p>` tags
- For off-schedule items, add `<p>[!BADGE Off schedule]{type=Neutral}</p>` after the link
- Empty `<p></p>` after the link is acceptable when no badge is needed
- Keep HTML indentation consistent with existing files

### Overview Trailing Sections

After all product area tables:

```markdown
## Release notes for other areas

### Workfront Fusion enhancements

New features in Workfront Fusion are available in Production at a cadence outside of the standard release schedule. For more information about the latest features, see [Adobe Workfront Fusion release activity](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Workfront Planning enhancements

New features in Workfront Planning are available in Production. For more information about the latest features, see [{Written Quarter} {Year} release activity for Adobe Workfront Planning](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-{YY}-q{N}.md).

There are no updates for the following at this point in the release:

* Scenario Planner
* Proof
* Goals

## Desktop proofing viewer updates

{Version info if available, otherwise omit section}

## Announcements

{Announcement content}

### API version {NN}

{API version info}

### Workfront Maintenance Updates

For information about the maintenance updates made during the {Written Quarter} {Year} release, see [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Training updates

Explore the latest updates made to learning programs, learning paths, videos, and guides for each Adobe Workfront product release. For more information, see the "What's New" section of the [Workfront Tutorials page](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html).
```

---

## Look and Feel Page Template

```markdown
---
title: Look-and-feel updates during the {Written Quarter} {Year} release time frame
description: Look-and-feel updates during the {Written Quarter} {Year} release time frame
author: {Author}
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: {existing UUID}
---

# Look-and-feel updates during the {Written Quarter} {Year} release time frame

This page describes minor updates to the look and feel of various areas of the Adobe Workfront application that were made within the {Written Quarter} {Year} release timeframe. These enhancements will be made available in the Production environment a minimum of 2 weeks after releasing to Preview.

For a list of all changes available with the {Written Quarter} {Year} release, see [{Written Quarter} {Year} Release overview](/help/quicksilver/product-announcements/product-releases/{YY}-q{N}-release-activity/{YY}-q{N}-release-overview.md).

## Feature Title

>[!NOTE]
>
>Preview release: {Month Day, Year}; Planned Production release: {Month Day, Year}

Description of the look-and-feel change.
```

---

## Date Callout Formats

### Product area pages (multi-line)

```markdown
>[!NOTE]
>
>Preview: March 5, 2026
>Production fast release: April 15, 2026
>Production for everyone: April 16, 2026
```

### Look-and-feel pages (single-line)

```markdown
>[!NOTE]
>
>Preview release: March 5, 2026; Planned Production release: March 19, 2026
```

### Weekly pages (single-line)

```markdown
>[!NOTE]
>
>Preview release: February 9, 2023; Planned Production release: February 23, 2023
```

---

## Known Inconsistencies to Watch For

1. **Wrong overview link quarter** — Product area pages sometimes link to the previous quarter's overview (e.g., `26-q1` instead of `26-q2`)
2. **Preview dates showing wrong year** — Overview tables sometimes show previous year in Preview column (e.g., "2025" instead of "2026")
3. **Missing closing `</tr>` tags** — Some HTML table rows lack proper closing tags
4. **`content-type: release-notes`** — Present in older files, omitted in newer 26-q2 product area pages. Follow the pattern of the current quarter.
5. **Typo in template** — The look-and-feel template has `relesae` instead of `release`; always use the correct spelling
6. **Missing `<p></p>` after feature link** — Some overview table rows omit the empty `<p>` tag after the `<a>` tag
