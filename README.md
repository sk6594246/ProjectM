# Stratega PM — User Guide & Workspace Manual

Welcome to **Stratega PM**, an enterprise-grade digital workspace engineered to streamline project execution, track timeline health, and optimize team resource distribution. Featuring a high-fidelity, responsive *Material Glass* visual shell, Stratega PM translates complex operational data into actionable visual insights across a unified 6-screen application ecosystem.

---

## 🧭 System Overview & The 6-Screen Layout

Stratega PM consolidates all project management vectors into an intuitive single-page ecosystem. You can transition seamlessly across the application using the global multi-panel navigation grid, which isolates views defensively to protect your active workspace state:

1. **Executive Operations Dashboard:** High-level status telemetry, critical path metrics, and automated system alerts.
2. **Interactive Kanban Board:** Task execution pipeline mapped out in intuitive operational stages.
3. **Dual-Baseline Gantt Timeline:** Interactive schedule engine mapping original plans against real-time project delivery.
4. **Strategic Analytics Engine:** Deep operational metrics, bottleneck indicators, and throughput performance.
5. **Team Resource Directory:** Cross-departmental matrix showing skill allocation, assignments, and availability.
6. **Workspace Administration Center:** Workflow configuration panels, automated baseline triggers, and custom data rules.

---

## 🔑 Security, Access, & Role-Based Permissions

Stratega PM enforces strict role-based workspace boundary walls while keeping daily interaction completely smooth. 

### Secure PIN-Based Access
* To log into your workspace profile, select your name from the directory dropdown and enter your unique, secure personal **Access PIN**. 
* The system uses an advanced cryptographic matching utility behind the scenes, ensuring unauthorized users cannot masquerade as team members or view proprietary project metrics.
* Session continuity is maintained by an integrated client-side persistence module, allowing you to refresh your browser without being forced to log back in constantly.

### Workspace Permissions Matrix
Your system role dictates what you can see and modify across the application:

| Feature/Action | Standard User | Department Manager | Workspace Admin |
| :--- | :--- | :--- | :--- |
| **Global Comments** | Read & Write (All Cards) | Read & Write (All Cards) | Read & Write (All Cards) |
| **Task Status Updates** | Authorized Departments Only | Authorized Departments Only | Global Access |
| **Task Creation & Editing** | Authorized Departments Only | Authorized Departments Only | Global Access |
| **Custom Status Workflows** | View Only | Modify (Own Projects) | Full Configuration |
| **Baseline Setting** | View Only | View Only | Full Modification |
| **Audit Log Auditing** | Hidden | View Only | Full Access |

*Note: Departmental boundaries ensure team members can only edit tasks belonging to their explicitly assigned departments (e.g., Engineering, Design, or Marketing), preventing accidental cross-contamination of project boards.*

---

## 📋 Mastering the Kanban Board

The Kanban Board is where tactical execution occurs. It presents your project lifecycle divided into status columns, facilitating smooth movement from conception to delivery.

```
+-------------------+  +-------------------+  +-------------------+  +-------------------+
|    TODO (03)      |  |  IN PROGRESS (02) |  |    REVIEW (01)    |  |    DONE (14)      |
+-------------------+  +-------------------+  +-------------------+  +-------------------+
| [Task #102]   [H] |  | [Task #94]    [M] |  | [Task #88]    [L] |  | [Task #72]    [M] |
| Core API Setup    |  | Design Wireframes |  | Copywriting Check |  | Schema Migration  |
| 💬 3 Comments      |  | 💬 0 Comments      |  | 💬 12 Comments    |  | ✅ Completed      |
+-------------------+  +-------------------+  +-------------------+  +-------------------+
```

### Navigating & Filtering Tasks
Locate what matters most using granular board controls at the top of the interface:
* **"Assigned to Me" Toggle:** Instantly hide all extraneous noise to focus strictly on your active load.
* **Priority Sorting:** Isolate cards marked as **High**, **Medium**, or **Low** priority.
* **One-Click Status Cycler:** Click the quick-action button right on a card to instantly shift it to the next logical phase in your workflow sequence without loading full details, or use the drop-down selector to move it immediately to any active stage.

### Interactive Task Modals & Optimistic UI
When you open a task card, create a new item, or submit edits, Stratega PM utilizes an asynchronous data sync process:
1. **Instant Updates:** Changes manifest on your screen immediately via local UI rendering.
2. **Background Synchronization:** The data updates securely over the network.
3. **Smart Cache Fallback:** If your network jitters or disconnects momentarily, the system locks your changes in a local browser cache and synchronizes them seamlessly once connectivity is re-established.

### Dynamic Inline Comment Capture
Keep communication contextual. You can read, write, and submit rich comments directly inside a task's interactive window. Comments are stored linearly and appear as a metric indicator badge directly on the main Kanban card face, prompting the wider team when active discussions are taking place.

---

## 📊 The Dual-Baseline Gantt Timeline

The Gantt Timeline engine provides a high-fidelity visual layout of project schedules. Uniquely, Stratega PM tracks **Dual-Baselines**, giving management a way to review how structural scope drift affects initial constraints over time.

```
Timeline Grid Mode: [ Day ] >>[ Week ]<< [ Month ]      Filters: Project [ Internal Systems ▼ ] Dept [ Eng ▼ ]
========================================================================================================================
TASK NAME            | W1-M   W1-T   W1-W   W1-T   W1-F   W1-S   W1-S | W2-M   W2-T   W2-W   W2-T   W2-F   W2-S   W2-S
------------------------------------------------------------------------------------------------------------------------
Database Provision   | [========================= Live Actual Progress =========================>
  - Baseline 1 (Target) | [-------------------------] 
  - Baseline 2 (Revised)|        [-------------------------]
------------------------------------------------------------------------------------------------------------------------
UI Wireframing       |                                                | [============== Live Actual Progress ===>
  - Baseline 1 (Target) |                                                | [-----------------]
  - Baseline 2 (Revised)|                                                |        [-------------------------]
========================================================================================================================
```

### Visualizing Baseline 1 vs. Baseline 2
* **Baseline 1 (Original Scope Target):** Represents the strict, original schedule benchmark agreed upon at project inception.
* **Baseline 2 (Revised Execution Vector):** Displays the secondary approved milestone target, accounting for changes in client requests or operational delays.
* **Live Execution Bar:** Placed stacked alongside the baseline metrics to visibly highlight schedule variances or delivery lag at a single glance.

### Interactive Timeline Controls
* **Granularity Toggle:** Instantly redraw the entire timeline layout. Switch gridlines between **Day**, **Week**, or **Month** views to alternate between micro-tracking and high-level milestone planning.
* **Timeline Scoping Filters:** Refine large project maps easily by filtering down metrics specifically by **Project Scope** or target **Operational Department**.
* **Theme Configuration:** Adjust structural color modes using a centralized multi-shade accent palette optimized for clear high-contrast print or low-light presentation reviews.

---

## 📈 Executive Analytics & Telemetry

The Analytics module tracks performance trends across your workspace, giving project leads empirical insight into delivery efficiency.

### Cumulative Monthly Throughput Waterfall
* Monitors the project's overall output speed over time. 
* Visualizes output volume using an additive waterfall engine, enabling managers to confirm whether real throughput velocity is matching long-term strategic projections.

### Cross-Departmental Workload Heatmaps
* Provides an operational view dividing tasks by department (Engineering, Design, Marketing, etc.).
* Displays data grids shaded by volume intensity, making it simple to spot departments that are overloaded before delays cascade down the production pipeline.

### "At-Risk" Resource Utilization Monitor
* Aggregates active team data to calculate total individual work loading.
* Flags team members whose total task counts, priority distributions, or work hours exceed optimal capacity limits, providing early warnings for potential burnout or resource constraints.

### "Time-in-State" Bottleneck Engine
* Automatically measures how long tasks hover in specific workflow stages (such as *Review* or *Quality Audit*).
* Visualizes this data through interactive charts, highlighting administrative bottlenecks where tasks sit idle waiting for sign-offs.

---

## ⚙️ Workspaces, Automations, & Auditing

Stratega PM balances flexible configuration options with robust quality controls.

### Smart Automation Rules
The system includes an intelligent relative-date automation manager that automatically updates task characteristics based on criteria you define. It uses flexible rules matching strings, booleans, and relative dates:
* **Dynamic Date Mappings:** If an automation sets a target date to `TODAY + 7` or `TODAY - 2`, the engine evaluates the current calendar day on the fly and inputs the correct date directly.
* **Automated Lifecycle Hooks:** Setting a task to "In Progress" or "Done" triggers automated lifecycle hooks, which automatically log precise timestamps for **Actual Start** and **Actual End** fields, preventing manual logging errors.

### Extensible Custom Status Workflows
Projects scale into specialized business domains naturally. Administrators can provision completely custom workflow paths per project, instantly establishing specialized operational steps:
* Standard Flow: `Todo` ➔ `In Progress` ➔ `Review` ➔ `Done`
* Extended Verticals: `Todo` ➔ `In Progress` ➔ **`Legal Review`** ➔ **`UAT Testing`** ➔ **`Quality Audit`** ➔ `Done`
The system scales horizontally, smoothly provisioning these custom fields across forms, filters, and Kanban boards.

### Deep Operation Audit Logger
Every modification, comment submission, status update, and schedule adjustment triggers a system-wide background audit logger. 
* This process compiles tracking data including timestamp records, modified task IDs, the acting user, and before/after values.
* The resulting records are sent to a dedicated database archive, providing managers and auditors with an immutable history of workspace activities for clear governance and transparency.
