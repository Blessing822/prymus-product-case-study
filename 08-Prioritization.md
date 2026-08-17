# PRYMUS — Product Prioritization

## 1. Overview

Product prioritization determines which features should be built first based on user value, business impact, urgency, dependencies, risk, and implementation effort.

For PRYMUS, prioritization was used to avoid attempting to build every requested capability simultaneously.

The approach focused on delivering the core operational value first:

> **Create → Assign → Execute → Track → Manage → Authorize**

This ensures that the MVP solves the primary workflow problem before expanding into advanced capabilities.

---

# 2. Prioritization Objectives

The prioritization process aims to:

- Deliver meaningful user value early.
- Validate the core product proposition.
- Reduce unnecessary development effort.
- Identify critical dependencies.
- Minimize product and implementation risk.
- Create a logical MVP.
- Enable incremental delivery.
- Leave room for learning and iteration.

---

# 3. Prioritization Framework

PRYMUS uses a combination of:

1. **RICE scoring**
2. **Impact vs. Effort**
3. **Dependency analysis**
4. **MVP validation**

No single framework was treated as an absolute decision-maker.

The final priority was based on both quantitative scoring and product judgment.

---

# 4. RICE Framework

RICE evaluates features using four factors:

### Reach

How many users or workflows are expected to benefit from the feature within a defined period?

### Impact

How significantly will the feature affect the user's ability to achieve their goal?

### Confidence

How confident are we in the reach and impact assumptions?

### Effort

How much development effort is required?

The RICE formula is:

```text
RICE Score = (Reach × Impact × Confidence) ÷ Effort

5. RICE Scoring Scale
Impact
Score	Meaning
3	Massive impact
2	High impact
1	Medium impact
0.5	Low impact
0.25	Minimal impact
Confidence
Score	Meaning
1.0	High confidence
0.8	Medium-high confidence
0.5	Medium confidence
0.3	Low confidence
Effort

Effort represents the relative amount of product, design, engineering, QA, and implementation work required.

For portfolio purposes, effort is represented using relative units rather than engineering hours.

6. PRYMUS RICE Prioritization
Feature	Reach	Impact	Confidence	Effort	RICE Score	Priority
Task Management	100	3	1.0	8	37.5	P0
Role & Permissions	100	3	1.0	7	42.9	P0
Kanban Board	90	3	0.9	5	48.6	P0
Workflow Management	85	3	0.9	7	32.8	P0
Authorization	70	3	0.9	6	31.5	P0
Notifications	80	2	0.8	4	32.0	P1
Calendar	70	2	0.8	4	28.0	P1
Collaboration	75	2	0.8	5	24.0	P1
Document Management	60	2	0.7	6	14.0	P1
Reporting & Analytics	50	2	0.6	7	8.6	P2

Note: The scores are relative prioritization estimates for the portfolio case study rather than production planning estimates.

7. Why Role & Permissions Comes First

Although the RICE score is not the only consideration, role and permission management is a foundational dependency.

PRYMUS has three major user groups:

Accounting Officer
Manager
Team Member

The Accounting Officer has organization-wide visibility and final authorization responsibility.

Managers manage teams and workflows.

Team Members execute assigned work.

Therefore, permission architecture needs to be established before implementing many downstream features.

8. Why Task Management Is Core

Task Management represents the foundation of the PRYMUS operational experience.

Users need to be able to:

Create tasks
Assign tasks
Define priorities
Set dates
Update status
Complete work
Track progress

Without task management, the Kanban Board, workflow tracking, worklogs, and authorization system would have limited value.

Therefore:

Task Management is a core MVP capability.

9. Why Kanban Was Prioritized

The Kanban Board was prioritized because it provides a simple visual representation of operational work.

Instead of requiring users to inspect individual tasks, users can immediately understand:

What needs to be done
What is currently being worked on
What is blocked
What has been completed

The Kanban Board also creates a visual management layer over the underlying Task Management system.

10. Kanban MVP Scope

The initial Kanban implementation focuses on:

To Do
   ↓
In Progress
   ↓
Blocked
   ↓
Completed

Core functionality:

View tasks
View task information
Move tasks
Update task status
Synchronize task status
Reflect workflow progress

Advanced filtering and reporting can be introduced later.

11. Why Workflow Management Was Prioritized

Individual tasks do not always represent the complete business process.

A workflow allows related tasks to be connected into a larger operational process.

For example:

Workflow
   │
   ├── Task 1
   ├── Task 2
   ├── Task 3
   └── Task 4

This enables Managers and Accounting Officers to understand not just individual tasks but the progress of the entire process.

12. Why Authorization Was Prioritized

PRYMUS includes an Accounting Officer role with final authorization responsibility.

This makes authorization a core part of the product rather than an optional administrative feature.

The basic authorization flow is:

Manager
   ↓
Submit for Authorization
   ↓
Accounting Officer
   ↓
Review
   ↓
Approve / Reject
   ↓
Task or Workflow Continues

This creates accountability and ensures that activities requiring final authorization cannot proceed without the appropriate decision.

13. Why Calendar Was Not P0

Calendar functionality is useful for scheduling and deadline visibility.

However, users can still create, assign, and complete tasks without a dedicated calendar.

Therefore, Calendar was classified as P1.

The product can validate the core task management experience before investing further in advanced scheduling capabilities.

14. Why Notifications Were Not P0

Notifications improve awareness but are not the fundamental mechanism through which work is created or completed.

The core workflow can function without a sophisticated notification system.

Therefore, notifications were prioritized after:

Task Management
Kanban
Workflow
Authorization

Notifications can then be introduced to improve adoption and operational responsiveness.

15. Why Analytics Were Prioritized Later

Analytics are valuable for understanding organizational performance.

However, meaningful analytics require sufficient product usage and reliable underlying data.

Building advanced reporting too early could create significant effort without enough validated usage data.

Therefore:

Data collection and core operational functionality come before advanced analytics.

Analytics can later measure:

Task completion
Overdue tasks
Workflow performance
Team workload
Authorization turnaround
Operational bottlenecks
16. Impact vs. Effort Analysis

Features were also evaluated using an Impact vs. Effort model.

Feature	Impact	Effort	Decision
Task Management	High	Medium	Build First
Role & Permissions	High	Medium	Build First
Kanban Board	High	Medium	Build First
Workflow	High	Medium-High	Build Early
Authorization	High	Medium	Build Early
Notifications	Medium	Low-Medium	Build Next
Calendar	Medium	Medium	Build Next
Collaboration	Medium	Medium	Build Next
Documents	Medium	High	Phase 2
Analytics	Medium	High	Phase 2
17. MVP Prioritization

The MVP focuses on five core capabilities:

1. User & Role Management

Establish secure role-based access.

2. Task Management

Enable users to create, assign, execute, and track work.

3. Kanban Board

Provide visual task management.

4. Workflow Management

Connect individual tasks to larger business processes.

5. Authorization

Allow the Accounting Officer to review and provide final authorization.

18. MVP User Journey

The prioritized MVP supports the following journey:

User logs in
      ↓
Role determines permissions
      ↓
Manager creates workflow
      ↓
Manager creates tasks
      ↓
Manager assigns tasks
      ↓
Team Member executes work
      ↓
Task moves through Kanban
      ↓
Workflow progress updates
      ↓
Manager submits for authorization
      ↓
Accounting Officer reviews
      ↓
Approve / Reject
      ↓
Workflow continues or returns for correction
19. Prioritization by Release
Release 1 — Core Foundation

Focus:

Authentication
User roles
Permissions
Task creation
Task assignment
Task status

Goal:

Establish the foundation for managing operational work.

Release 2 — Visual Work Management

Focus:

Kanban Board
Task cards
Drag-and-drop/status movement
Task status synchronization
Basic filters

Goal:

Make operational work visible and easier to manage.

Release 3 — Workflow & Authorization

Focus:

Workflow creation
Task-to-workflow association
Workflow progress
Authorization requests
Accounting Officer review
Approval/rejection

Goal:

Connect task execution with organizational processes and final authorization.

Release 4 — Operational Efficiency

Focus:

Calendar
Notifications
Comments
Worklogs
Document integration

Goal:

Improve collaboration and operational efficiency.

Release 5 — Insights

Focus:

Task analytics
Workflow analytics
Performance metrics
Bottleneck identification
Management reporting

Goal:

Enable data-driven operational decision-making.

20. Prioritization Trade-offs

Prioritization requires making trade-offs.

For PRYMUS, the following decisions were made:

Build core task functionality before advanced reporting.

Reason:

The product needs reliable operational data before meaningful analytics can be generated.

Build Kanban before advanced visualization.

Reason:

Kanban directly improves day-to-day task visibility and requires less complexity than a full analytics layer.

Build authorization before advanced automation.

Reason:

Authorization is directly connected to the organization's operational control model.

Delay advanced document capabilities.

Reason:

Basic document association supports the workflow, while advanced document functionality can be introduced after the core workflow is validated.

21. Dependency-Based Prioritization

Some features cannot provide their full value without other capabilities.

Roles & Permissions
        ↓
Task Management
        ↓
Kanban Board
        ↓
Workflow Management
        ↓
Authorization
        ↓
Notifications
        ↓
Analytics

This dependency structure influenced the delivery sequence.

22. Prioritization Principles

The following principles guided prioritization:

1. Solve the core problem first

Prioritize features that directly address the primary user problem.

2. Build the smallest useful version

Avoid adding complexity before validating the core experience.

3. Consider dependencies

A feature should not be prioritized without considering what it depends on.

4. Optimize for learning

Early releases should generate useful product feedback.

5. Balance user and business value

Features should provide meaningful value to users while supporting organizational objectives.

6. Use evidence where available

Prioritization should increasingly rely on:

User feedback
Usage data
Task completion rates
Adoption
Operational performance
Stakeholder feedback
23. Prioritization Decision Matrix
Feature	User Value	Business Value	Dependency	Effort	Final Priority
Role Management	High	High	Foundational	Medium	P0
Task Management	High	High	Foundational	Medium	P0
Kanban	High	High	Task Management	Medium	P0
Workflow	High	High	Task Management	Medium-High	P0
Authorization	High	High	Workflow	Medium	P0
Notifications	Medium	Medium	Core workflow	Medium	P1
Calendar	Medium	Medium	Task dates	Medium	P1
Collaboration	Medium	Medium	Tasks	Medium	P1
Documents	Medium	High	Permissions	High	P1
Analytics	Medium	High	Historical data	High	P2
24. How Prioritization Should Evolve

Priorities should not remain static.

After each release, the product team should evaluate:

What users adopted
What users ignored
Where users encountered friction
Which workflows were completed successfully
Which tasks remained overdue
Where users dropped off
Which features generated the most value
Which assumptions were incorrect

These insights should feed back into the backlog.

Build
 ↓
Measure
 ↓
Learn
 ↓
Reprioritize
 ↓
Build
25. Success Metrics After Prioritization

The success of the prioritized roadmap should be evaluated using measurable outcomes.

Task Management
Task creation rate
Task completion rate
Task completion time
Overdue task rate
Kanban
Kanban adoption
Status update frequency
Time spent in each status
Blocked task rate
Workflow
Workflow completion rate
Workflow cycle time
Workflow bottleneck rate
Authorization
Authorization turnaround time
Approval rate
Rejection rate
Time from submission to decision
Overall Product
Active users
Feature adoption
Workflow completion
User retention
Task completion efficiency
26. Prioritization Outcome

The prioritization process resulted in a focused MVP rather than attempting to deliver every possible feature simultaneously.

The core product sequence is:

Secure Access
     ↓
Task Management
     ↓
Kanban
     ↓
Workflow
     ↓
Authorization
     ↓
Collaboration
     ↓
Scheduling
     ↓
Analytics

This approach allows PRYMUS to establish its core operational value first and expand based on validated user needs and product data.

27. Product Manager Reflection

The key product management principle behind this prioritization exercise is:

The most important feature is not necessarily the feature with the most requests. It is the feature that creates the greatest validated value while supporting the product's strategic objective.

Prioritization therefore requires balancing:

User Value + Business Value + Evidence + Effort + Dependencies + Risk

rather than simply building the largest number of features.

🔐 Confidentiality Note

Some product details have been generalized or omitted to respect confidentiality and protect proprietary information.

This case study focuses on the product management approach to prioritization, trade-offs, MVP definition, dependency analysis, and roadmap decision-making, rather than confidential company information.



### Your GitHub portfolio now looks like this


```text
PRYMUS Product Case Study
│
├── README.md
├── 01-Product-Overview.md
├── 02-Problem-Statement.md
├── 03-User-Research.md
├── 04-PRD.md
├── 05-User-Stories.md
├── 06-Acceptance-Criteria.md
├── 07-Product-Backlog.md
└── 08-Prioritization.md        ← ✅
