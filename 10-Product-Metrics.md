# PRYMUS — Product Metrics & Measurement Framework

## 1. Overview

Product metrics provide a framework for measuring whether PRYMUS is creating meaningful value for its users and achieving its business objectives.

The goal is not simply to measure how many features are being used.

The goal is to understand whether PRYMUS is helping organizations:

- Create work efficiently
- Assign responsibilities clearly
- Complete tasks faster
- Monitor operational progress
- Manage workflows effectively
- Reduce bottlenecks
- Improve authorization processes
- Increase organizational visibility

The measurement approach therefore focuses on **outcomes rather than feature delivery alone.**

---

# 2. Product Measurement Philosophy

The product team should continuously answer five questions:

1. Are users adopting PRYMUS?
2. Are they successfully completing their core workflows?
3. Are PRYMUS features improving operational efficiency?
4. Are users continuing to use the product?
5. Is the product creating measurable organizational value?

The measurement loop is:

```text
Build
  ↓
Instrument
  ↓
Measure
  ↓
Analyze
  ↓
Learn
  ↓
Improve
  ↓
Build Again

3. North Star Metric
Proposed North Star Metric
Successfully Completed Authorized Workflows

This metric represents the number of workflows that are:

Created
Assigned
Executed
Completed
Authorized where authorization is required

within a defined period.

Why this metric?

PRYMUS is not simply a task management application.

Its broader value is helping organizations move operational work from initiation to completion with visibility and accountability.

A workflow that successfully reaches completion represents the successful execution of organizational work.

Therefore:

Successfully Completed Authorized Workflows is a strong candidate for the PRYMUS North Star Metric.

4. North Star Metric Formula
Successfully Completed Authorized Workflows
=
Completed Workflows
that have passed all required authorization steps

For workflows that do not require authorization:

Completed Workflow = Successful Workflow

For workflows requiring authorization:

Completed
      +
Required Authorization
      =
Successful Workflow
5. Supporting Metric Framework

The North Star Metric is supported by several metric categories:

Acquisition
     ↓
Activation
     ↓
Engagement
     ↓
Task Completion
     ↓
Workflow Completion
     ↓
Authorization
     ↓
Retention
     ↓
Business Value
6. Acquisition Metrics

Acquisition measures how users and organizations enter the product.

Potential metrics include:

New organizations onboarded
New users invited
Invitation acceptance rate
Account creation rate
Organization activation rate
Example
Invitation Acceptance Rate
=
Accepted Invitations ÷ Total Invitations Sent × 100
Why it matters

If users are not successfully entering the product, downstream product metrics cannot grow.

7. Activation Metrics

Activation measures whether a new user reaches the product's initial value.

Proposed activation event

A new organization is considered activated when it:

Adds users
Creates a workflow
Creates at least one task
Assigns the task
Begins execution
Activation Rate
Activated Organizations
÷
New Organizations
× 100
Why it matters

Account creation alone does not demonstrate product value.

Activation should represent the point at which users begin experiencing the core PRYMUS workflow.

8. Task Management Metrics

Task Management is a core PRYMUS capability.

Key metrics include:

Tasks created
Tasks assigned
Tasks started
Tasks completed
Task completion rate
Overdue task rate
Blocked task rate
Average task completion time
Task Completion Rate
Completed Tasks
÷
Total Tasks Due
× 100
Goal

Measure whether users are successfully moving work to completion.

9. Task Completion Time

Task completion time measures the time between when a task enters execution and when it is completed.

Task Completion Time
=
Completion Timestamp
-
Start Timestamp
Why it matters

A reduction in task completion time may indicate improved operational efficiency.

10. Overdue Task Rate
Overdue Task Rate
=
Overdue Tasks
÷
Total Tasks
× 100
Why it matters

A high overdue rate could indicate:

Poor workload distribution
Unrealistic deadlines
Process bottlenecks
Lack of visibility
Resource constraints

This metric should therefore be used as a diagnostic signal rather than simply a performance score.

11. Blocked Task Rate
Blocked Task Rate
=
Blocked Tasks
÷
Active Tasks
× 100
Why it matters

Blocked tasks can reveal operational bottlenecks.

The Product Manager can investigate:

Why tasks are blocked
How long they remain blocked
Which workflows generate the most blockers
Which teams experience the most blockers
12. Kanban Metrics

The Kanban Board should be measured based on whether it improves work visibility and task management.

Key metrics:

Kanban adoption rate
Tasks moved between statuses
Status update frequency
Average time in each status
Blocked task duration
Completed tasks through Kanban
Kanban Adoption
Users Using Kanban
÷
Active Users
× 100
Why it matters

This determines whether users are adopting visual task management.

13. Time in Status

Measure how long tasks remain in each Kanban state.

Example:

To Do → 2 days
In Progress → 4 days
Blocked → 1 day
Completed
Why it matters

Long durations in a particular status can identify workflow friction.

For example:

If tasks consistently remain in "Blocked" for several days, the product team should investigate the underlying process.

14. Workflow Metrics

Key workflow metrics include:

Workflows created
Workflows started
Workflows completed
Workflow completion rate
Workflow cycle time
Workflow abandonment rate
Workflow bottleneck rate
Workflow Completion Rate
Completed Workflows
÷
Started Workflows
× 100
Why it matters

This is one of the most important indicators of whether PRYMUS is helping organizations complete operational processes.

15. Workflow Cycle Time
Workflow Cycle Time
=
Workflow Completion Date
-
Workflow Start Date
Goal

Track whether organizations can complete processes more efficiently over time.

16. Authorization Metrics

Authorization is a core PRYMUS capability because the Accounting Officer has final authorization responsibility.

Key metrics include:

Authorization requests submitted
Authorization requests reviewed
Approval rate
Rejection rate
Average authorization turnaround time
Pending authorization count
Authorization backlog
17. Authorization Turnaround Time
Authorization Turnaround Time
=
Decision Timestamp
-
Submission Timestamp
Why it matters

Long authorization delays can become operational bottlenecks.

The product team can investigate whether delays are caused by:

Too many pending requests
Lack of notifications
Insufficient information
Approval workflow complexity
Accounting Officer workload
18. Authorization Approval Rate
Approval Rate
=
Approved Requests
÷
Total Decided Requests
× 100

The approval rate should not be treated as a standalone measure of success.

A high rejection rate may indicate:

Poor task quality
Missing information
Incorrect workflow setup
Unclear authorization requirements

Therefore, the metric should be combined with qualitative feedback.

19. Retention Metrics

Retention measures whether users continue using PRYMUS after initial adoption.

Key metrics:

Weekly Active Users
Monthly Active Users
Organization retention
User retention
Returning users
Workflow reuse
Task creation frequency
20. Weekly Active Users
WAU
=
Unique users who perform a meaningful product action
within a 7-day period

Meaningful actions may include:

Creating a task
Updating a task
Completing a task
Moving a Kanban card
Creating a workflow
Reviewing authorization
Approving a request
21. Feature Adoption

Feature adoption measures whether users are using the functionality the product team has invested in.

Examples:

Task Management
Users Creating Tasks
÷
Active Users
× 100
Kanban
Users Using Kanban
÷
Active Users
× 100
Workflow
Users Creating Workflows
÷
Eligible Users
× 100
Authorization
Authorization Requests Processed
÷
Authorization Requests Created
× 100
22. Product Funnel

The PRYMUS core product funnel can be represented as:

User Invited
     ↓
Account Activated
     ↓
Workflow Created
     ↓
Task Created
     ↓
Task Assigned
     ↓
Task Started
     ↓
Task Completed
     ↓
Workflow Completed
     ↓
Authorization Completed

The Product Manager can analyze conversion between each stage.

23. Funnel Analysis

Example:

Funnel Stage	Users/Workflows	Conversion
Organizations Onboarded	100	100%
Activated	80	80%
Created Workflow	70	87.5%
Created Task	65	92.9%
Started Task	58	89.2%
Completed Task	50	86.2%
Completed Workflow	42	84.0%

The numbers above are illustrative and should not be interpreted as actual PRYMUS performance data.

24. Metrics by User Role

Different users should have different success indicators.

Accounting Officer

Primary metrics:

Authorization turnaround time
Pending authorization count
Workflow visibility
Organizational completion rate
Overdue task visibility
Bottleneck identification
Manager

Primary metrics:

Tasks created
Tasks assigned
Task completion rate
Overdue task rate
Workflow completion
Blocked task rate
Team workload
Team Member

Primary metrics:

Assigned tasks
Task completion rate
Task completion time
Overdue tasks
Blocked tasks
Status updates
25. Product Health Dashboard

A high-level management dashboard could contain:

┌─────────────────────────────────────┐
│          PRODUCT HEALTH             │
├─────────────────────────────────────┤
│ Active Organizations                │
│ Active Users                        │
│                                     │
│ Task Completion Rate                │
│ Workflow Completion Rate            │
│                                     │
│ Overdue Task Rate                   │
│ Blocked Task Rate                   │
│                                     │
│ Authorization Turnaround Time       │
│ Pending Authorizations              │
└─────────────────────────────────────┘

This dashboard gives the Accounting Officer and management a high-level view of operational health.

26. Product Metrics Hierarchy

Metrics should be organized into three levels.

Level 1 — North Star

Successfully Completed Authorized Workflows

Level 2 — Product Outcomes
Workflow completion rate
Task completion rate
Authorization turnaround
Workflow cycle time
Overdue task rate
Level 3 — Feature Metrics
Kanban adoption
Task creation
Task updates
Calendar usage
Notification engagement
Comment usage
Document usage

This prevents the team from optimizing individual feature usage without understanding the broader product outcome.

27. Metrics and Product Decisions

Metrics should lead to product decisions.

For example:

Observation

Blocked task rate increases.

Investigation

Analyze:

Which workflows are affected?
Which teams are affected?
How long are tasks blocked?
What reasons are recorded?
Product Decision

Potential actions could include:

Improve task dependency visibility
Add blocker reasons
Improve notifications
Introduce escalation mechanisms
Improve workflow design
28. Example Product Experiment
Hypothesis

Providing clearer Kanban visibility will help Managers identify blocked work faster.

Experiment

Introduce improved blocked-task visibility on the Kanban Board.

Primary Metric

Average time a task remains blocked.

Secondary Metrics
Blocked task resolution rate
Workflow completion rate
Manager Kanban adoption
Success Criteria

A successful experiment would demonstrate a meaningful reduction in blocked-task duration without negatively affecting other workflow metrics.

29. Metrics Instrumentation

Important product events should be tracked.

Example events:

user_signed_up
user_invited
workflow_created
task_created
task_assigned
task_started
task_status_changed
task_blocked
task_completed
kanban_viewed
kanban_task_moved
authorization_submitted
authorization_approved
authorization_rejected
workflow_completed

Each event should capture relevant properties such as:

User ID
Organization ID
Role
Workflow ID
Task ID
Timestamp
Previous status
New status
30. Data Quality Considerations

Product metrics are only useful when the underlying data is reliable.

The product team should ensure:

Events are consistently named.
Events are fired at the correct point.
Duplicate events are prevented.
Required properties are captured.
Timestamps are accurate.
User and organization identifiers are consistent.
Historical data remains interpretable after product changes.
31. Metrics Review Cadence
Weekly

Review:

Active users
Task activity
Task completion
Blocked tasks
Authorization backlog
Critical product issues
Monthly

Review:

Retention
Feature adoption
Workflow completion
Operational efficiency
Product trends
Quarterly

Review:

North Star Metric
Product strategy
Business outcomes
Major roadmap assumptions
Customer feedback
Product-market signals
32. Metrics Ownership

The Product Manager should work with cross-functional teams to ensure metrics are understood and acted upon.

Product
Defines metrics
Interprets trends
Connects metrics to product decisions
Engineering
Implements event tracking
Ensures data reliability
Supports instrumentation
Design
Investigates UX friction
Uses behavioral insights to improve experiences
Leadership
Reviews business-level outcomes
Provides strategic direction
33. Leading vs. Lagging Indicators

PRYMUS should track both leading and lagging indicators.

Leading Indicators

These can indicate future product outcomes:

Task creation
Workflow creation
Kanban adoption
User engagement
Status updates
Lagging Indicators

These show realized outcomes:

Workflow completion
Task completion
Retention
Reduced cycle time
Reduced overdue tasks
Authorization efficiency

The product team should avoid relying exclusively on leading indicators.

34. Metrics Guardrails

Optimizing one metric can sometimes negatively affect another.

For example:

Increasing task completion rate should not result in users prematurely marking tasks as completed.

Therefore, supporting guardrail metrics may include:

Task reopening rate
Authorization rejection rate
User satisfaction
Workflow error rate
Data quality issues

This helps ensure that improvements represent genuine product value.

35. Example Metrics Scorecard
Metric	Category	Frequency	Owner
Completed Authorized Workflows	North Star	Monthly	Product
Task Completion Rate	Outcome	Weekly	Product
Workflow Completion Rate	Outcome	Weekly	Product
Authorization Turnaround	Outcome	Weekly	Product
Overdue Task Rate	Health	Weekly	Product
Blocked Task Rate	Health	Weekly	Product
Kanban Adoption	Feature	Monthly	Product
Workflow Adoption	Feature	Monthly	Product
WAU	Engagement	Weekly	Product
Retention	Business	Monthly	Product
36. Product Success Definition

PRYMUS should be considered successful when users consistently use the platform to move operational work from initiation to completion.

Success should therefore be demonstrated through:

Increasing workflow completion
Increasing task completion
Reducing operational delays
Improving visibility
Reducing blocked work
Improving authorization turnaround
Sustaining user adoption
Increasing organizational reliance on PRYMUS
37. Continuous Improvement Framework

Metrics should feed directly into product discovery and prioritization.

Metrics
   ↓
Identify Problem
   ↓
Investigate Cause
   ↓
Generate Solutions
   ↓
Prioritize
   ↓
Experiment
   ↓
Measure Impact
   ↓
Scale / Iterate / Remove

This creates a continuous improvement cycle.

38. Product Manager Reflection

A strong product metrics strategy should answer more than:

"How many people used the feature?"

It should answer:

"Did the feature improve the user's ability to accomplish an important outcome?"

For PRYMUS, this means moving beyond feature-level usage and measuring whether the platform helps organizations complete work more efficiently, maintain visibility, and enforce accountability.

The objective is therefore not simply to maximize activity.

The objective is to maximize meaningful completed work.

39. Confidentiality Note

Some product details have been generalized or omitted to respect confidentiality and protect proprietary information.

This case study focuses on the product management approach to metrics definition, product analytics, experimentation, outcome measurement, and continuous improvement, rather than confidential company information.



### Your complete PRYMUS case-study portfolio is now:


```text
prymus-product-case-study/
│
├── README.md
│
├── 01-Product-Overview.md
├── 02-Problem-Statement.md
├── 03-User-Research.md
├── 04-PRD.md
├── 05-User-Stories.md
├── 06-Acceptance-Criteria.md
├── 07-Product-Backlog.md
├── 08-Prioritization.md
├── 09-Roadmap.md
└── 10-Product-Metrics.md
