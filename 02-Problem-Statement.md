# PRYMUS — Problem Statement

## 1. Problem Overview

Organizations often manage their operational activities across disconnected tools, spreadsheets, emails, messaging platforms, physical documents, and manual approval processes.

As the number of tasks, workflows, documents, and employees increases, this fragmented approach makes it difficult for organizations to maintain visibility, accountability, and control over their operations.

PRYMUS addresses this problem by providing a centralized platform where **workflows, tasks, documents, collaboration, and authorization** can be managed and monitored within one system.

---

# 2. The Core Problem

The core problem is:

> **Organizations lack a centralized and structured way to create, assign, execute, monitor, review, and authorize operational work across different levels of the organization.**

This creates gaps between:

* Executives and managers
* Managers and team members
* Tasks and workflows
* Documents and operational activities
* Task execution and final authorization

As a result, managers may struggle to understand the current state of their team's work, while executives may lack a clear organization-wide view of operational activities.

---

# 3. Who Experiences the Problem?

The problem affects multiple user groups.

## Accounting Officer / Executive

The Accounting Officer needs visibility across the organization but may face challenges such as:

* Limited visibility into ongoing tasks
* Difficulty monitoring multiple managers
* Difficulty tracking workflow progress
* Lack of centralized activity history
* Difficulty identifying delayed or blocked work
* Difficulty reviewing activities requiring authorization
* Reliance on managers to provide operational updates

---

## Managers

Managers need to coordinate teams and ensure work is completed correctly.

Common challenges include:

* Creating and assigning tasks manually
* Tracking multiple tasks across different tools
* Difficulty understanding team workload
* Limited visibility into task progress
* Difficulty identifying overdue tasks
* Difficulty identifying blocked tasks
* Scattered task-related communication
* Difficulty maintaining a clear record of task activity
* Difficulty escalating tasks for higher-level authorization

---

## Team Members

Team members need clarity about the work assigned to them.

Potential challenges include:

* Unclear task ownership
* Missing or incomplete task information
* Difficulty understanding deadlines
* Difficulty tracking their workload
* Scattered task-related communication
* Difficulty knowing the current status of work
* Lack of centralized access to supporting documents

---

# 4. Current-State Challenges

Before a centralized workflow and task management solution, operational activities may be distributed across different tools and processes.

A typical process may look like:

```text
Manager identifies work
        ↓
Task communicated through email/chat
        ↓
Employee executes work
        ↓
Progress communicated manually
        ↓
Manager follows up
        ↓
Documents exchanged separately
        ↓
Manager reviews work
        ↓
Executive is contacted for authorization
        ↓
Completion recorded manually
```

This process can create unnecessary delays and information gaps.

---

# 5. Key Pain Points

## 5.1 Lack of Centralized Task Management

Tasks may be created and tracked through different channels.

This makes it difficult to answer basic questions such as:

* What tasks are currently active?
* Who is responsible for each task?
* What is the priority?
* When is the task due?
* What is blocking the task?
* Has the task been completed?

---

## 5.2 Poor Visibility

Managers may not have a real-time overview of their team's workload.

Executives may have even less visibility because information is often communicated through periodic reports or individual updates.

This can make it difficult to identify operational issues early.

---

## 5.3 Fragmented Communication

Task-related conversations can occur across:

* Email
* Messaging applications
* Meetings
* Phone calls
* Documents
* Spreadsheets

When communication is disconnected from the task itself, important context can become difficult to find.

---

## 5.4 Difficulty Tracking Progress

Without a visual task management system, users may struggle to understand how work is progressing.

A Kanban Board can address this by providing a visual representation of work:

```text
TO DO → IN PROGRESS → BLOCKED → COMPLETED
```

This allows users to quickly understand the state of work.

---

## 5.5 Weak Accountability

When tasks do not have clearly defined owners, deadlines, priorities, and statuses, accountability becomes difficult.

A structured task record can provide:

* Assignee
* Priority
* Start date
* Due date
* Status
* Workflow
* Comments
* Worklog
* History

This creates a clearer record of responsibility.

---

## 5.6 Inefficient Authorization

Some organizational activities require approval from a higher level of authority.

Without a structured authorization workflow, these activities may depend on manual communication.

This can create:

* Delays
* Unclear approval status
* Difficulty tracking authorization
* Limited auditability
* Risk of unauthorized completion

PRYMUS addresses this through a role-based authorization structure in which the Accounting Officer can provide final authorization where required.

---

# 6. Root Causes

The major root causes identified include:

### Fragmented Tools

Different activities are managed in different systems.

### Manual Processes

Tasks, approvals, and progress updates may depend heavily on manual communication.

### Lack of Centralized Visibility

There is no single source of truth for organizational work.

### Unstructured Task Tracking

Tasks may not consistently contain ownership, priority, deadlines, and status.

### Limited Workflow Integration

Tasks and documents may not be connected to the broader business workflow.

### Weak Authorization Tracking

Approval processes may not have a clear digital trail.

---

# 7. Problem Statement by User

### Accounting Officer

> **I need organization-wide visibility and control over operational activities so that I can monitor managers, review important activities, and provide final authorization when required.**

### Manager

> **I need a centralized way to create, assign, prioritize, and monitor tasks so that I can effectively manage my team and ensure workflows are completed on time.**

### Team Member

> **I need clear visibility into my assigned tasks, deadlines, and requirements so that I can complete my work efficiently and keep my manager informed of my progress.**

---

# 8. Product Opportunity

The identified problems create an opportunity to build a centralized operational management platform that connects:

```text
Tasks
  +
Workflows
  +
Documents
  +
Collaboration
  +
Authorization
  +
Reporting
```

into one product experience.

PRYMUS can create a single source of truth for organizational activities while providing different levels of visibility and control based on user roles.

---

# 9. Proposed Product Direction

PRYMUS addresses the problem through several connected capabilities.

### Centralized Task Management

Provide one place to create, assign, track, and manage work.

### Kanban Board

Provide visual visibility into task progress.

### Calendar View

Provide date-based visibility into deadlines and workload.

### Workflow Execution

Connect individual tasks to larger operational processes.

### Document Management

Keep relevant documents connected to workflows and tasks.

### Collaboration

Keep task-related communication connected to the relevant work.

### Role-Based Authorization

Ensure users have appropriate access and authorization based on their organizational responsibilities.

### Executive Oversight

Give the Accounting Officer organization-wide visibility and the ability to monitor and authorize activities where required.

---

# 10. Desired Future State

The desired experience is:

```text
Workflow Created
       ↓
Tasks Defined
       ↓
Tasks Assigned
       ↓
Team Members Execute
       ↓
Progress Updated
       ↓
Manager Monitors
       ↓
Accounting Officer Reviews
       ↓
Final Authorization
       ↓
Task Completed
       ↓
Workflow Completed
```

Each stage should be traceable within PRYMUS.

---

# 11. Product Success Criteria

The problem can be considered successfully addressed when PRYMUS enables organizations to:

* Centralize operational tasks
* Clearly assign responsibility
* Improve task visibility
* Reduce manual follow-ups
* Track work in real time
* Identify overdue and blocked tasks
* Improve manager oversight
* Provide executive-level visibility
* Improve authorization tracking
* Maintain task and workflow history
* Connect tasks with relevant documents
* Improve overall workflow efficiency

---

# 12. Key Product Hypotheses

### Hypothesis 1 — Centralized Task Management

> If organizations have a centralized task management system, then managers will spend less time manually tracking work and following up with team members.

### Hypothesis 2 — Kanban Visibility

> If users can visually track tasks through a Kanban Board, then they will identify blocked, overdue, and in-progress work more quickly.

### Hypothesis 3 — Executive Visibility

> If the Accounting Officer has organization-wide visibility, then executive oversight and decision-making will become more informed and efficient.

### Hypothesis 4 — Structured Authorization

> If authorization is built into the workflow, then organizations will have clearer approval processes and better traceability.

### Hypothesis 5 — Connected Workflows

> If tasks, documents, and workflows are connected, then users will spend less time searching for information and coordinating work across disconnected systems.

---

# 13. Product Problem Summary

PRYMUS is fundamentally solving a **visibility, accountability, coordination, and authorization problem**.

The product moves organizations from:

> **Fragmented → Centralized**

> **Manual → Structured**

> **Limited Visibility → Real-Time Visibility**

> **Unclear Accountability → Clear Ownership**

> **Disconnected Approvals → Structured Authorization**

> **Reactive Management → Proactive Oversight**

The goal is not simply to provide another task management tool, but to create a connected operational environment where **work can be assigned, executed, monitored, reviewed, authorized, and completed within a structured workflow.**

---

##  Confidentiality Note

Some product details have been generalized or omitted to respect confidentiality and protect proprietary information.

This case study focuses on my **product management approach, problem framing, decision-making, and product thinking** rather than confidential business information.
