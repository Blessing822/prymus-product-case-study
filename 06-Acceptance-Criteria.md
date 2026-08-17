# PRYMUS — Acceptance Criteria

## 1. Overview

This document defines the acceptance criteria for key PRYMUS features.

Acceptance criteria describe the conditions that must be satisfied for a feature or user story to be considered complete and ready for release.

The criteria use the **Given / When / Then** format where appropriate.

---

# 2. Task Management

## AC-TM-001 — Create Task

**Related User Story:** US-MGR-001

### Acceptance Criteria

**Scenario 1 — Successful task creation**

- **Given** a Manager has permission to create tasks
- **When** the Manager selects "Create Task"
- **Then** the system should display the task creation form.

**And**

- The Manager should be able to enter:
  - Task name
  - Description
  - Assignee
  - Priority
  - Start date
  - Due date
  - Workflow

**And**

- **When** the Manager submits the form with all required information
- **Then** the system should create the task successfully.

**And**

- The task should appear in the appropriate task list and Kanban Board.

---

## AC-TM-002 — Required Task Information

**Related User Story:** US-MGR-001

### Acceptance Criteria

- **Given** a Manager is creating a task
- **When** a required field is empty
- **Then** the system should prevent submission.

**And**

- The system should clearly identify the missing information.

---

# 3. Task Assignment

## AC-TM-003 — Assign Task

**Related User Story:** US-MGR-003

### Acceptance Criteria

- **Given** a Manager is creating or editing a task
- **When** the Manager selects an eligible team member
- **Then** the selected user should become the task assignee.

**And**

- The task should display the assigned user.

**And**

- The assigned user should be able to see the task in their task list.

---

## AC-TM-004 — Reassign Task

**Related User Story:** US-MGR-011

### Acceptance Criteria

- **Given** a Manager has permission to reassign a task
- **When** the Manager selects a new assignee
- **Then** the task should be assigned to the new user.

**And**

- The system should record the reassignment in task history.

**And**

- The previous assignee should no longer be responsible for the task.

---

# 4. Task Priority

## AC-TM-005 — Set Priority

**Related User Story:** US-MGR-004

### Acceptance Criteria

- **Given** a Manager is creating or editing a task
- **When** the Manager selects a priority
- **Then** the task should display the selected priority.

Supported priority levels should include:

- Low
- Medium
- High
- Critical

---

# 5. Task Dates

## AC-TM-006 — Set Start and Due Date

**Related User Story:** US-MGR-005 / US-MGR-006

### Acceptance Criteria

- **Given** a Manager is creating or editing a task
- **When** the Manager enters a start date and due date
- **Then** the dates should be saved against the task.

**And**

- The due date should be visible to authorized users.

---

## AC-TM-007 — Overdue Task

### Acceptance Criteria

- **Given** a task has a due date
- **And** the due date has passed
- **And** the task has not been completed
- **Then** the system should identify the task as overdue.

**And**

- The task should remain visible to the appropriate Manager and Accounting Officer.

---

# 6. Task Status

## AC-TM-008 — Update Task Status

**Related User Story:** US-TM-005

### Acceptance Criteria

- **Given** a Team Member has permission to update a task
- **When** the Team Member changes the task status
- **Then** the new status should be saved.

Supported statuses should include:

```text
To Do
In Progress
Blocked
Completed
And

The status change should be reflected on the Kanban Board.

And

The change should be recorded in task history.
7. Blocked Tasks
AC-TM-009 — Mark Task as Blocked

Related User Story: US-TM-006

Acceptance Criteria
Given a Team Member cannot continue working on a task
When the Team Member marks the task as "Blocked"
Then the task status should change to "Blocked".

And

The Manager should be able to identify the task as blocked.

And

The status change should be recorded in task history.
8. Complete Task
AC-TM-010 — Complete Task

Related User Story: US-TM-011

Acceptance Criteria
Given a Team Member has completed the required work
When the Team Member marks the task as completed
Then the task status should change to "Completed".

And

The Manager should be able to see that the task has been completed.

And

The completion should be recorded in task history.

And

If the task requires authorization, the system should not treat the task as fully completed until the required authorization has been completed.
9. Kanban Board
AC-KB-001 — View Kanban Board

Related User Story: US-KB-001

Acceptance Criteria
Given an authorized user opens the Kanban Board
Then the system should display tasks organized by status.

The default columns should be:

To Do
In Progress
Blocked
Completed
AC-KB-002 — Task Card Information

Related User Story: US-KB-002

Acceptance Criteria

Each task card should display:

Task name
Assignee
Priority
Due date
Workflow
Status
10. Kanban Task Movement
AC-KB-003 — Move Task Between Columns

Related User Story: US-KB-003

Acceptance Criteria
Given an authorized user is viewing the Kanban Board
When the user moves a task from one permitted column to another
Then the task status should be updated.

And

The task should immediately appear in the new column.

And

The underlying task record should reflect the new status.

And

The status change should be recorded in task history.
AC-KB-004 — Unauthorized Status Change
Acceptance Criteria
Given a user does not have permission to modify a task
When the user attempts to change its status
Then the system should prevent the change.

And

The existing task status should remain unchanged.
11. Workflow Management
AC-WF-001 — Create Workflow

Related User Story: US-MGR-016

Acceptance Criteria
Given a Manager has workflow creation permission
When the Manager selects "Create Workflow"
Then the system should display the workflow creation form.

The Manager should be able to provide:

Workflow name
Description
Owner
Start date
Due date

And

The system should create the workflow after successful submission.
12. Add Task to Workflow
AC-WF-002 — Associate Task With Workflow

Related User Story: US-MGR-017

Acceptance Criteria
Given a workflow exists
When a Manager creates or edits a task
Then the Manager should be able to associate the task with the workflow.

And

The task should appear within the workflow.

And

The workflow should include the task when calculating progress.
13. Workflow Progress
AC-WF-003 — Calculate Workflow Progress

Related User Story: US-MGR-019

Acceptance Criteria
Given a workflow contains multiple tasks
When tasks change status
Then the workflow progress should update accordingly.

And

Users with permission should be able to see the current workflow progress.
14. Workflow Synchronization
AC-WF-004 — Task Status Synchronization
Acceptance Criteria
Given a task is associated with a workflow
When the task status changes
Then the system should update the relevant workflow progress.

And

The task and workflow should remain synchronized.
15. Calendar
AC-CAL-001 — View Tasks on Calendar

Related User Story: US-CAL-001

Acceptance Criteria
Given an authorized user opens Calendar View
Then the system should display relevant tasks according to their dates.

And

Tasks should display their relevant start and due dates.
AC-CAL-002 — View Task From Calendar

Related User Story: US-CAL-004

Acceptance Criteria
Given a task appears on the calendar
When an authorized user selects the task
Then the system should open the task details.
AC-CAL-003 — Identify Overdue Tasks
Acceptance Criteria
Given a task has passed its due date
And the task is not completed
Then the calendar should identify the task as overdue.
16. Comments
AC-COL-001 — Add Comment

Related User Story: US-COL-001

Acceptance Criteria
Given a user has permission to comment on a task
When the user enters a comment and submits it
Then the comment should be added to the task.

And

The comment should display the author's identity and timestamp.
AC-COL-002 — View Comments

Related User Story: US-COL-002

Acceptance Criteria
Given a user has permission to access the task
When the user opens the task
Then they should be able to view relevant comments.
17. Worklog
AC-WL-001 — Add Worklog

Related User Story: US-COL-003

Acceptance Criteria
Given a user has permission to add worklogs
When the user records work performed
Then the system should save the worklog against the task.

The worklog should contain:

User
Date
Time spent
Work performed
Notes where applicable
AC-WL-002 — View Worklog
Acceptance Criteria
Given an authorized user opens a task
When the user selects the worklog
Then the system should display relevant worklog entries.
18. Task History
AC-HIST-001 — Record Task Changes

Related User Story: US-HIST-001

Acceptance Criteria

The system should automatically record important task changes including:
Task creation
Assignment
Reassignment
Status change
Priority change
Due date change
Comment
Authorization request
Authorization decision
Completion
AC-HIST-002 — Identify User and Timestamp

Related User Story: US-HIST-003

Acceptance Criteria

Each relevant history entry should contain:

Action
User responsible
Date
Time
AC-HIST-003 — View Task History

Related User Story: US-HIST-002

Acceptance Criteria
Given an authorized user opens a task
When the user accesses task history
Then the system should display recorded activities in chronological order.
19. Authorization
AC-AUTH-001 — Submit Authorization Request

Related User Story: US-AUTH-001

Acceptance Criteria
Given a Manager has completed the required task or workflow stage
When the Manager submits the activity for authorization
Then the authorization status should change to "Pending".

And

The Accounting Officer should be able to see the request.
20. Accounting Officer Review
AC-AUTH-002 — View Pending Authorization

Related User Story: US-AUTH-002

Acceptance Criteria
Given an authorization request is pending
When the Accounting Officer opens the authorization section
Then the pending request should be displayed.

And

The Accounting Officer should be able to access relevant task and workflow information.
AC-AUTH-003 — Review Authorization Details

Related User Story: US-AUTH-003

Acceptance Criteria

The Accounting Officer should be able to review:

Task details
Workflow information
Assignee
Current status
Comments
Worklogs
Relevant documents
Task history

before making a decision.

21. Approve Authorization
AC-AUTH-004 — Approve Request

Related User Story: US-AUTH-004

Acceptance Criteria
Given an authorization request is pending
When the Accounting Officer selects "Approve"
Then the authorization status should change to "Approved".

And

The system should record the Accounting Officer who approved the request.

And

The system should record the date and time.

And

The relevant task or workflow should proceed to the next stage.
22. Reject Authorization
AC-AUTH-005 — Reject Request

Related User Story: US-AUTH-005

Acceptance Criteria
Given an authorization request is pending
When the Accounting Officer selects "Reject"
Then the system should require a reason or comment.

And

The authorization status should change to "Rejected".

And

The rejection should be recorded in history.

And

The relevant Manager should be able to see the rejection reason.
23. Authorization Status
AC-AUTH-006 — View Authorization Status

Related User Story: US-AUTH-006

Acceptance Criteria

A Manager should be able to see whether a request is:

Not Submitted
Pending
Approved
Rejected
24. Authorization History
AC-AUTH-007 — Record Authorization Decision

Related User Story: US-AUTH-007

Acceptance Criteria

Each authorization decision should record:

Decision
Decision maker
Date
Time
Reason/comment where applicable

The record should not be editable by unauthorized users.

25. Authorization and Task Completion
AC-AUTH-008 — Prevent Unauthorized Completion
Acceptance Criteria
Given a task requires final authorization
When the task is submitted for authorization
Then the task should remain in an appropriate authorization state.

And

The task should not be treated as fully completed until the Accounting Officer provides the required authorization.
26. Document Management
AC-DOC-001 — Upload Document

Related User Story: US-DOC-001

Acceptance Criteria
Given a user has permission to upload documents
When the user uploads a supported document
Then the document should be stored successfully.

And

The document should be associated with the relevant task or workflow.
AC-DOC-002 — Access Supporting Document

Related User Story: US-TM-009

Acceptance Criteria
Given a document is associated with a task
And the user has permission to access the document
When the user opens the task
Then the document should be accessible.
AC-DOC-003 — Unauthorized Document Access
Acceptance Criteria
Given a user does not have permission to access a document
When the user attempts to access it
Then the system should deny access.
27. Role-Based Access Control
AC-ROLE-001 — Accounting Officer Permissions
Acceptance Criteria

The Accounting Officer should be able to:

View organizational workflows
View organizational tasks
Monitor managers
Monitor teams
Review authorization requests
Approve authorization requests
Reject authorization requests
Access relevant task history
Access relevant worklogs
Create tasks where permitted
AC-ROLE-002 — Manager Permissions
Acceptance Criteria

Managers should be able to:

Create workflows
Create tasks
Assign tasks
Update permitted task information
Monitor team tasks
Use the Kanban Board
View relevant calendar activities
Review worklogs
Review task history
Submit activities for authorization
AC-ROLE-003 — Team Member Permissions
Acceptance Criteria

Team Members should be able to:

View assigned tasks
View task details
Update permitted task statuses
Add comments
Add worklogs
Access permitted documents
Complete assigned work
AC-ROLE-004 — Unauthorized Action
Acceptance Criteria
Given a user attempts to perform an action outside their permissions
When the action is submitted
Then the system should prevent the action.

And

The system should display an appropriate permission message.
28. Notifications
AC-NOT-001 — Task Assignment Notification
Acceptance Criteria
Given a Manager assigns a task
When the task is successfully assigned
Then the assignee should receive an appropriate notification.
AC-NOT-002 — Authorization Notification
Acceptance Criteria
Given a Manager submits a task for authorization
When the request is successfully submitted
Then the Accounting Officer should receive an appropriate notification.
AC-NOT-003 — Authorization Decision Notification
Acceptance Criteria
Given the Accounting Officer approves or rejects a request
When the decision is recorded
Then the relevant Manager should receive an appropriate notification.
29. Search and Filtering
AC-SEARCH-001 — Filter Tasks
Acceptance Criteria

Authorized users should be able to filter tasks by relevant fields such as:

Assignee
Status
Priority
Workflow
Due date
Authorization status

The displayed results should reflect the selected filters.

30. Cross-Module Acceptance Criteria
AC-CROSS-001 — Task and Workflow Synchronization
Acceptance Criteria
A task associated with a workflow must remain linked to that workflow.
Changes to relevant task statuses should be reflected in workflow progress.
Removing or changing the task association should update the workflow appropriately.
AC-CROSS-002 — Task and Authorization Synchronization
Acceptance Criteria
Authorization requests must remain linked to their originating task or workflow.
Approval decisions must update the relevant authorization status.
Relevant task/workflow states must reflect the authorization decision.
AC-CROSS-003 — Task and Document Association
Acceptance Criteria
Documents associated with a task must remain accessible from the task.
Access must respect user permissions.
Document activity should be traceable where required.
31. Auditability
AC-AUDIT-001 — Record Important Actions

The system should maintain an audit trail for important activities.

Examples include:

Login where required
Task creation
Task assignment
Task reassignment
Status changes
Authorization decisions
Document actions
Permission-sensitive activities
32. Error Handling
AC-ERR-001 — Failed Task Creation
Given a user attempts to create a task
When the system encounters an error
Then the system should inform the user that the task was not created.

And

The user should be able to retry without losing entered information where technically possible.
AC-ERR-002 — Failed Status Update
Given a user changes a task status
When the update fails
Then the system should communicate the failure.

And
The task should retain its previous confirmed status.
33. Acceptance Criteria Quality Standards

Acceptance criteria should be:

Clear

The expected behavior should be easy to understand.

Testable

QA should be able to verify whether the criteria have been met.

Specific

Criteria should avoid ambiguous language.

User-Focused

The criteria should reflect the intended user outcome.

Independent Where Possible

Each criterion should focus on a specific behavior.

Traceable

Each criterion should connect back to a product requirement or user story.

34. Requirements Traceability

The acceptance criteria establish a connection between:

User Problem
     ↓
User Need
     ↓
User Story
     ↓
Acceptance Criteria
     ↓
Development
     ↓
QA Testing
     ↓
Release

This ensures that product development remains connected to the original user problem.

35. Definition of Done

A user story is considered complete when:

All acceptance criteria pass.
The implementation matches the approved requirements.
QA testing is completed.
Critical and high-severity defects are resolved.
Role permissions have been validated.
Relevant activity is recorded where required.
The feature works for all applicable user roles.
Product/design/engineering stakeholders have reviewed the implementation.
The feature is ready for release.

🔐 Confidentiality Note

Some product details have been generalized or omitted to respect confidentiality and protect proprietary information.

This case study focuses on the product management process, requirements definition, acceptance criteria, and decision-making approach rather than confidential company information.
