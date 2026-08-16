# PRYMUS — User Research

## 1. Research Overview

Product discovery for PRYMUS focused on understanding how organizations manage operational workflows, assign tasks, monitor progress, collaborate on work, and handle authorization.

The research objective was to identify the biggest friction points in the existing process and translate those insights into product opportunities.

The research focused on three primary user groups:

* Accounting Officers / Executives
* Managers
* Team Members

---

# 2. Research Objectives

The research aimed to understand:

1. How organizations currently manage tasks and workflows.
2. How managers assign and monitor work.
3. How team members receive and execute tasks.
4. How executives monitor organizational activities.
5. How users track task progress.
6. How users manage deadlines and priorities.
7. How users communicate around tasks.
8. How documents are connected to operational activities.
9. How authorization and approval processes work.
10. What information users need to make effective decisions.

---

# 3. Research Questions

### General Workflow

* How are operational workflows currently created?
* What happens after a workflow is initiated?
* Who is responsible for each stage?
* How is workflow progress monitored?

### Task Management

* How are tasks created?
* Who assigns tasks?
* How are tasks prioritized?
* How are deadlines communicated?
* How do users know what they are expected to complete?
* How is task completion tracked?

### Management & Oversight

* How do managers monitor their teams?
* How do managers identify overdue tasks?
* How do managers identify blocked work?
* What information does an executive need to monitor organizational activities?

### Collaboration

* Where do users communicate about tasks?
* How are updates shared?
* How do users access supporting documents?

### Authorization

* Which activities require authorization?
* Who provides final authorization?
* How is approval status currently tracked?
* What happens when an activity is rejected?

---

# 4. User Groups

## 👑 Accounting Officer / Executive

### Primary Goals

* Maintain organization-wide visibility
* Monitor managers and teams
* Review important activities
* Track organizational progress
* Provide final authorization
* Identify operational bottlenecks

### Key Needs

* Organization-wide dashboard
* Visibility across workflows
* Visibility across tasks
* Manager activity monitoring
* Authorization requests
* Task and workflow history
* Performance information

---

## 👨🏽‍💼 Managers

### Primary Goals

* Coordinate team activities
* Assign work
* Monitor progress
* Ensure deadlines are met
* Manage workflows
* Escalate activities requiring authorization

### Key Needs

* Task creation
* Task assignment
* Priorities
* Start and due dates
* Kanban Board
* Calendar View
* Task history
* Worklogs
* Comments
* Workflow visibility

---

## 👩🏽‍💻 Team Members

### Primary Goals

* Understand assigned work
* Complete tasks
* Meet deadlines
* Communicate progress
* Access relevant information

### Key Needs

* Personal task view
* Task details
* Deadlines
* Priorities
* Status updates
* Comments
* Worklogs
* Supporting documents

---

# 5. Current-State User Journey

The existing operational process can involve several disconnected steps.

```text
Work Identified
      ↓
Manager Communicates Task
      ↓
Team Member Receives Task
      ↓
Task Executed
      ↓
Progress Communicated
      ↓
Manager Reviews
      ↓
Additional Follow-up
      ↓
Authorization Requested
      ↓
Executive Reviews
      ↓
Work Completed
```

### Identified Friction

At several points in this journey, information can become fragmented.

For example:

* Task details may be communicated separately from documents.
* Progress updates may depend on manual follow-up.
* Managers may not have a real-time view of workload.
* Executives may depend on managers for operational updates.
* Authorization may occur outside the workflow.
* There may be limited visibility into historical task activity.

---

# 6. Key Research Insights

## Insight 1 — Users Need a Single Source of Truth

Operational information becomes difficult to manage when tasks, documents, communication, and workflow information are distributed across multiple channels.

### Product Implication

PRYMUS should centralize relevant operational information.

---

## Insight 2 — Managers Need Better Work Visibility

Managers need to quickly understand:

* What is pending?
* What is in progress?
* What is blocked?
* What is overdue?
* Who is responsible?

### Product Implication

A visual Kanban Board and structured task management system should be core product capabilities.

---

## Insight 3 — Executives Need Organization-Wide Visibility

The Accounting Officer needs a broader view than an individual manager.

### Product Implication

The Accounting Officer should have organization-wide visibility into tasks, workflows, activities, and authorization requests.

---

## Insight 4 — Tasks Need Clear Ownership

Every task should have a clearly defined responsible person.

### Product Implication

Task assignment should be a core capability.

Each task should clearly display:

* Assignee
* Priority
* Status
* Start date
* Due date
* Workflow

---

## Insight 5 — Users Need Multiple Ways to View Work

Different users manage work differently.

Managers may prefer a visual Kanban Board, while users managing deadlines may prefer a calendar.

### Product Implication

PRYMUS should provide both:

* Kanban View
* Calendar View

---

## Insight 6 — Task Context Should Remain Connected

Users need access to relevant communication, documents, and activity history without searching across multiple systems.

### Product Implication

Tasks should support:

* Comments
* Worklogs
* Task history
* Supporting documents

---

## Insight 7 — Authorization Needs to Be Structured

Some activities require final approval from a higher-level authority.

### Product Implication

PRYMUS should incorporate authorization into the workflow rather than treating approval as a separate process.

---

# 7. User Needs

Based on the research, the following user needs were identified.

### Accounting Officer Needs

* See all organizational workflows
* See all organizational tasks
* Monitor managers
* Monitor team activities
* Review authorization requests
* Track workflow progress
* Access relevant activity history
* Make final authorization decisions

### Manager Needs

* Create tasks
* Assign tasks
* Set priorities
* Set deadlines
* Monitor team workload
* Track task progress
* Identify blocked work
* Identify overdue work
* Review task history
* Escalate activities for authorization

### Team Member Needs

* See assigned tasks
* Understand task requirements
* Know deadlines
* Update task status
* Communicate progress
* Record work performed
* Access relevant documents

---

# 8. User Personas

## Persona 1 — Accounting Officer

**Role:** Executive / Organization-wide Oversight

**Primary Goal:** Maintain visibility and control over organizational operations.

**Pain Points:**

* Limited visibility into daily activities
* Dependence on managers for updates
* Difficulty tracking multiple workflows
* Manual authorization processes

**Success Looks Like:**

> Having a centralized view of organizational activities and being able to review and authorize important activities efficiently.

---

## Persona 2 — Manager

**Role:** Department / Team Manager

**Primary Goal:** Coordinate team activities and ensure work is completed on time.

**Pain Points:**

* Manual task tracking
* Difficulty monitoring workload
* Scattered updates
* Difficulty identifying blocked work
* Repeated follow-ups

**Success Looks Like:**

> Being able to see what each team member is working on, identify issues quickly, and keep workflows moving.

---

## Persona 3 — Team Member

**Role:** Operational Employee

**Primary Goal:** Complete assigned work efficiently.

**Pain Points:**

* Unclear task requirements
* Scattered information
* Difficulty tracking deadlines
* Lack of visibility into task expectations

**Success Looks Like:**

> Knowing exactly what needs to be done, when it is due, and how to communicate progress.

---

# 9. User Journey — Manager

```text
Login
  ↓
View Dashboard
  ↓
Review Workflows
  ↓
Create / Select Workflow
  ↓
Create Task
  ↓
Assign Team Member
  ↓
Set Priority & Deadline
  ↓
Monitor Kanban Board
  ↓
Review Progress
  ↓
Identify Blocked / Overdue Tasks
  ↓
Review Completed Work
  ↓
Submit for Authorization if Required
```

---

# 10. User Journey — Team Member

```text
Login
  ↓
View Assigned Tasks
  ↓
Open Task
  ↓
Review Requirements
  ↓
Access Supporting Documents
  ↓
Begin Work
  ↓
Update Status
  ↓
Add Comments / Worklog
  ↓
Complete Task
  ↓
Manager Reviews
```

---

# 11. User Journey — Accounting Officer

```text
Login
  ↓
View Organization Dashboard
  ↓
Monitor Workflows
  ↓
Monitor Tasks
  ↓
Review Manager Activities
  ↓
Identify Pending Authorization
  ↓
Review Task / Workflow Information
  ↓
Approve or Reject
  ↓
Authorization Recorded
  ↓
Workflow Progress Updated
```

---

# 12. Research-to-Product Mapping

The research findings were translated into product capabilities.

| User Need                   | Product Response        |
| --------------------------- | ----------------------- |
| Centralized task management | Task Management         |
| Visual progress tracking    | Kanban Board            |
| Deadline management         | Calendar View           |
| Clear ownership             | Task Assignment         |
| Task context                | Comments & Worklogs     |
| Historical visibility       | Task History            |
| Executive oversight         | Accounting Officer Role |
| Operational management      | Manager Role            |
| Task execution              | Team Member Role        |
| Structured approvals        | Authorization Workflow  |
| Centralized information     | Document Management     |
| Connected processes         | Workflow Execution      |

---

# 13. Prioritized User Problems

Based on their impact on operational efficiency and visibility, the major problems can be prioritized as:

### High Priority

1. Lack of centralized task management
2. Limited visibility into task progress
3. Difficulty assigning and tracking responsibility
4. Lack of executive-level visibility
5. Unstructured authorization processes

### Medium Priority

6. Fragmented task communication
7. Difficulty tracking deadlines
8. Limited task history
9. Difficulty accessing supporting documents

### Lower Priority

10. Additional visualization and reporting capabilities

This prioritization provides a foundation for subsequent product prioritization.

---

# 14. Product Opportunities Identified

The research highlighted several opportunities:

### Opportunity 1

Create a centralized task management system.

### Opportunity 2

Introduce a Kanban Board to make work visually understandable.

### Opportunity 3

Provide calendar-based task management.

### Opportunity 4

Give managers better visibility into team activities.

### Opportunity 5

Give the Accounting Officer organization-wide oversight.

### Opportunity 6

Connect tasks to workflows and documents.

### Opportunity 7

Build authorization directly into operational workflows.

### Opportunity 8

Create a traceable history of task and workflow activities.

---

# 15. Research Conclusion

The research indicates that PRYMUS should not be positioned simply as a task management tool.

The broader opportunity is to create an **operational workflow management platform** that connects:

**People + Tasks + Workflows + Documents + Collaboration + Authorization**

within a single system.

The research findings directly informed the product requirements, task management capabilities, Kanban Board, role hierarchy, authorization model, and workflow design.

---

## 🔐 Confidentiality Note

Some research details have been generalized to respect confidentiality and protect proprietary information.

This case study focuses on the **research approach, user needs, product insights, and how research findings informed product decisions** rather than confidential user or company information.
