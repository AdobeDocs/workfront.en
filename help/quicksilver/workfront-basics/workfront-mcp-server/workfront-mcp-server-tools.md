---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Adobe Workfront MCP server tools
description: Reference list of the tools available through the Adobe Workfront MCP server, grouped by Workfront area.
author: Courtney
feature: Get Started with Workfront
hide: true
---

# Adobe Workfront MCP server tools

This article lists the tools that the [!DNL Adobe Workfront] MCP server exposes to a connected AI agentic platform. The platform calls these tools on your behalf when you ask it to find, create, update, or delete Workfront items.

Tools are grouped by Workfront area: Approvals, Planning, and Workflow.

For information about how to use these tools through an AI agentic platform, see [Use the Adobe Workfront MCP server](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md). For information about how to set up the connection, see [Configure the Adobe Workfront MCP server](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

>[!IMPORTANT]
>
>The AI agentic platform acts in Workfront using your Workfront account, access level, and object permissions. A tool only works if you have the corresponding access in Workfront. Adobe is not responsible for changes the AI agentic platform makes to your Workfront data.

## Approvals tools (23 total)

### Documents

<!-- 
VERIFY BEFORE PUBLISHING: The following three tools may not be customer-facing. If engineering confirms they're internal-only, delete these rows from the table below:
- approvals_get_document_by_version_id
- approvals_list_aem_linked_folders
- approvals_send_documents_to_aem_folder
-->

| Title | Tool name | What it does |
|---|---|---|
| Find document version by name | `approvals_find_document_version_by_name` | Looks up a document's current version ID by filename. Supports partial matches. |
| Get document by version ID | `approvals_get_document_by_version_id` | Fetches document details (name, size, upload date, uploader) for a known document version ID. |
| Get documents by project | `approvals_get_documents_by_project` | Lists documents inside a Workfront project, with each document's current version ID. |
| Resolve document scope | `approvals_resolve_document_scope` | Expands a project or folder into the list of document version IDs it contains. Supports project, folder, and folder-by-name scopes. |
| List AEM-linked folders | `approvals_list_aem_linked_folders` | Lists Workfront document folders that are linked to Adobe Experience Manager. |
| Send documents to AEM folder | `approvals_send_documents_to_aem_folder` | Moves one or more Workfront documents to an AEM-linked folder. |

### Approval workflows

| Title | Tool name | What it does |
|---|---|---|
| Get approval workflow info | `approvals_get_approval_info` | Returns the current approval workflow (stages, participants, status) for a document version. |
| Create or update approval workflow | `approvals_create_or_update_approval_workflow` | Creates or updates the approval workflow stages for a document version. Supports linear and parallel (graph) stage dependencies. |
| Create approval from template | `approvals_create_approval_from_template` | Creates an approval workflow on a document using an existing template. |
| Request document approval | `approvals_request_document_approval` | Opens a guided form for requesting approval on a document version (title, approvers/reviewers, optional due date and message). |
| Delete approval stage | `approvals_delete_approval_stage` | Deletes a single stage from an approval workflow by name or position. Only not-started stages can be deleted. |

### Reminders

| Title | Tool name | What it does |
|---|---|---|
| Send reminder to participants | `approvals_send_reminder_to_participants` | Sends reminder emails to specific participants in an approval stage. Works only for started, not-completed, not-locked stages. |
| Send reminder to undecided participants | `approvals_send_reminder_to_undecided` | Sends reminder emails to all undecided participants (notified, opened, or commented) in an approval stage. |

### Approval templates

| Title | Tool name | What it does |
|---|---|---|
| List approval templates | `approvals_list_templates` | Lists approval templates available in this Workfront instance. Supports filtering by creator, participant, and sorting by usage. |
| Search template by name | `approvals_search_template_by_name` | Finds approval templates by name (case-insensitive partial match). |
| Create approval template | `approvals_create_template` | Creates a new approval template with linear or graph-based stage dependencies. |
| Update approval template | `approvals_update_template` | Updates an existing template with structured modifications (add or remove participants, rename stages, set deadlines, etc.). |

### Lookups and users

| Title | Tool name | What it does |
|---|---|---|
| Get current user | `approvals_get_current_user` | Returns the calling user's Workfront identity, including name, user ID, home team name, and home team ID. |
| Find user by name | `approvals_find_user_by_name` | Looks up a Workfront user's ID by name (fuzzy or partial match). Returns name, ID, email, title, and avatar URL. |
| Find team by name | `approvals_find_team_by_name` | Looks up a Workfront team's ID by name (fuzzy or partial match). |
| Find project by name | `approvals_find_project_by_name` | Looks up Workfront projects by partial name match across the system. |
| Get projects by owner | `approvals_get_projects_by_owner` | Lists Workfront projects where the calling user is the owner. |
| Get Adobe region | `approvals_get_adobe_region` | Returns the Adobe name of a cloud provider region. |

## Planning tools (43 total)

### Workspaces

| Title | Tool name | What it does |
|---|---|---|
| Get workspace | `planning_get_workspace` | Retrieves full details of a workspace by ID or alias. |
| Get workspace list | `planning_get_workspace_list` | Lists all available workspaces with cursor-based pagination. |
| Create workspace | `planning_create_workspace` | Creates a new empty workspace to organize record types, fields, and data. |
| Create workspace from template | `planning_create_workspace_from_template` | Creates a new workspace pre-populated using an existing template. |
| Update workspace | `planning_update_workspace` | Partially updates a workspace — name, description, icon, sections, or owner. |
| Delete workspace | `planning_delete_workspace` | Permanently deletes a workspace and all its data. |
| Convert workspace to template | `planning_convert_workspace_to_template` | Saves an existing workspace as a reusable template (requires admin). |
| Get workspace sharing | `planning_get_workspace_sharing` | Returns the current sharing and permissions configuration for a workspace. |
| Modify workspace sharing | `planning_modify_workspace_sharing` | Updates who has access to a workspace and at what permission level. |

### Record types

| Title | Tool name | What it does |
|---|---|---|
| Get record type | `planning_get_record_type` | Fetches full details of a record type including its fields and views. |
| Create record types | `planning_create_record_types` | Creates one or more record types within a workspace section. |
| Update record type | `planning_update_record_type` | Partially updates a record type's name, description, icon, or color. |
| Delete record type | `planning_delete_record_type` | Permanently deletes a record type and all its records, fields, and views. |
| List global record types | `planning_list_global_record_types` | Lists all centrally-defined (global) record types visible to the current user. |
| List addable global record types | `planning_list_addable_global_record_types` | Lists global record types that can be added to a specific workspace. |
| Add global record type to workspace | `planning_add_global_record_type_to_workspace` | Links a global record type into a specified workspace. |
| Remove global record type from workspace | `planning_remove_global_record_type_from_workspace` | Unlinks a global record type from a workspace; deletes all its records in that workspace. |
| Get external record workspaces | `planning_get_external_record_workspaces` | Finds which workspaces and record types are connected to a specific external record. |
| Get record type sharing | `planning_get_record_type_sharing` | Returns the sharing and permissions for a specific record type. |
| Modify record type sharing | `planning_modify_record_type_sharing` | Updates who can access a record type and at what permission level. |

### Records

| Title | Tool name | What it does |
|---|---|---|
| Get record | `planning_get_record` | Retrieves full details of a single record by ID. |
| Search records | `planning_search_records` | Searches and filters records within a record type. |
| Bulk record actions | `planning_bulk_record_actions` | Creates, updates, deletes, or restores multiple records in a single request. |
| Create connection record | `planning_create_connection_record` | Creates a new record in a connected external system (for example, a Workfront project). |
| Update records order | `planning_update_records_order` | Changes the display order of records within a record type. |
| Get record change log | `planning_get_record_change_log` | Returns the field-level edit history for a record. |
| Get record sharing | `planning_get_record_sharing` | Returns the sharing configuration for a specific record. |
| Modify records sharing | `planning_modify_records_sharing` | Updates who can access one or more records and at what permission level. |

### Fields

| Title | Tool name | What it does |
|---|---|---|
| Get field | `planning_get_field` | Retrieves full details and value schema for a field by ID. |
| Create fields | `planning_create_fields` | Adds one or more fields (columns) to a record type. |
| Update field | `planning_update_field` | Partially updates a field's name, description, options, or configuration. |
| Delete field | `planning_delete_field` | Permanently removes a field and all its data from a record type. |

### Views

| Title | Tool name | What it does |
|---|---|---|
| Get view | `planning_get_view` | Returns complete details of a view by ID. |
| Create view | `planning_create_view` | Creates a new table, timeline, or calendar view for a record type. |
| Update view | `planning_update_view` | Partially updates an existing view's configuration, filters, or sorting. |
| Delete view | `planning_delete_view` | Permanently deletes a view (records are not affected). |
| Get view sharing | `planning_get_view_sharing` | Returns the sharing configuration for a specific view. |
| Modify view sharing | `planning_modify_view_sharing` | Updates who can access a view and at what permission level. |

### Templates

| Title | Tool name | What it does |
|---|---|---|
| Get template list | `planning_get_template_list` | Lists all available workspace templates with summary info. |
| Get template | `planning_get_template` | Retrieves full details of a specific template by ID. |

### Search & utilities

| Title | Tool name | What it does |
|---|---|---|
| Search resources | `planning_search_resources` | Searches across workspaces, record types, and views by name. |
| Search sharing data | `planning_search_sharing_data` | Finds users, groups, teams, roles, and companies by name for sharing and permissions. |
| Search users | `planning_search_users` | Searches for users with pagination support. |

## Workflow tools (5 total)

Workflow tools are the general-purpose actions the AI agentic platform uses to work with any Workfront object — projects, tasks, issues, hours, assignments, programs, portfolios, and so on.

| Title | Tool name | What it does |
|---|---|---|
| Search objects | `workflow_search_any_object` | Searches for Workfront objects with flexible filter parameters, ordering, and pagination. |
| Create object | `workflow_create_any_object` | Creates a new Workfront object such as a project, task, issue, hour, assignment, program, or portfolio. |
| Update object | `workflow_update_any_object` | Updates fields on an existing Workfront object. |
| Delete object | `workflow_delete_any_object` | Deletes a Workfront object by ID. Requires explicit user confirmation before the action is performed. |
| Resolve field names | `workflow_resolve_field_names_any_object` | Converts user-provided field names or labels to the underlying Workfront API field names so the AI agentic platform can build accurate requests. |

## How tools are updated

When Adobe releases a new version of the Workfront MCP server, the AI agentic platform uses the new tool set automatically. You don't need to reconnect or change anything on your side.
