# Database Isolation Level Simulator (C# / WinForms)

This project is a **C# WinForms simulation tool** that demonstrates how different
**SQL transaction isolation levels** affect concurrency behavior, execution flow,
and deadlock risk.

The system runs concurrent operations from two user types (Type A / Type B),
logs each thread step-by-step, measures execution time, and detects deadlocks.

---

## 🎯 Purpose
The goal is to provide a practical, visual way to observe:
- How isolation levels impact concurrent access
- How conflicts appear as errors or blocks
- When deadlocks are more likely to occur
- The performance trade-offs between isolation levels

---

## 🧩 How It Works
- The user selects the number of concurrent workers for **Type A** and **Type B**
- An **isolation level** is selected from the UI
- The simulation starts and logs:
  - Thread ID
  - User type (A/B)
  - Step number
  - Status (OK / ERROR / INFO)
  - Execution time summary
  - Deadlock detection (YES/NO)

---

## 🖥 Screenshots

### 1) Application UI (Start)
![Start UI](images/01_ui_start.png)

### 2) READ UNCOMMITTED – Example Run
![Read Uncommitted](images/02_read_uncommitted_run.png)

### 3) READ COMMITTED – Example Error/Conflict
![Read Committed](images/03_read_committed_error.png)

### 4) REPEATABLE READ – Timing Output Example
![Repeatable Read](images/04_repeatable_read_timing.png)

### 5) SERIALIZABLE – Deadlock Example
![Serializable Deadlock](images/05_serializable_deadlock.png)

---

## 🛠 Tech Stack
- C# (WinForms)
- Visual Studio
- SQL transaction concepts (isolation levels, concurrency, deadlocks)
- Thread-based simulation + logging

---

## 📌 Notes
This project is primarily focused on **concurrency behavior and transaction theory**.
UI design is intentionally kept simple to emphasize correctness and traceability.

---

## 📄 Report
Detailed explanation and design documentation:

`report/SE308_term_project_report.pdf`
