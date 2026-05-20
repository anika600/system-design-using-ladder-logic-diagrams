## 🚀 Overview
The goal of these projects was to transition traditional hardware-based relay logic into programmable, fail-safe software solutions. Each project emphasizes **safety interlocking**, **fault diagnostics**, and **process efficiency**.

## 🛠 Featured Projects

### 1. Motor Control with Safety Feedback
* **Problem:** Standard motor starters lack verification. If a contactor fails or a belt breaks, the system may not know the motor is stationary.
* **Solution:** Implemented a "Safety Timeout" logic. If the system commands a start but doesn't receive a physical feedback signal within 5 seconds, the system triggers an emergency shutdown.
* **Key Logic:** Latching circuits, On-delay timers for feedback monitoring, and manual fault reset.

### 2. Fail-Safe Valve Monitoring (Dual-State)
* **Problem:** Process valves can get stuck mid-travel, which is hazardous in chemical or fluid transport.
* **Solution:** A robust monitoring system for "Open" and "Closed" positions. It identifies specific failures (e.g., "Failure to Open" vs. "Failure to Close") and prevents further operation until the error is cleared.
* **Key Logic:** Dual-path timer diagnostics and hardware-software interlocking.

### 3. Four-Way Sequential Traffic Controller
* **Problem:** Managing complex intersections requires precise timing and the absolute prevention of conflicting "Green" signals.
* **Solution:** A synchronized four-phase controller using a cascading timer sequence. It includes a clearance interval logic (All-Red) and uses internal memory markers to manage complex state transitions.
* **Key Logic:** Cascading timers, internal memory markers (M-bits), and safety conflict prevention.

---

## 💻 Technical Stack
* **Software:** Siemens LOGO! Soft Comfort V8.x
* **Hardware Target:** Siemens LOGO! 8 Logic Modules
* **Language:** Ladder Diagram (LAD)

## 📂 File Structure
* `/*.lld`: Original LOGO! Soft Comfort project files.
* `/Screenshots`: Visual representations of the Ladder Logic rungs.
* `/Documentation`: Detailed I/O mapping and project descriptions.

### How to View
**Quick View (Recommended):** Simply navigate to the /Screenshots folder in this repository. I have provided images of the Ladder Diagrams for each project so you can review the logic directly in your browser.

OR
1. Download and install **Siemens LOGO! Soft Comfort**.
2. Clone this repository: `git clone https://github.com/YourUsername/ProjectName.git`
3. Open the `.lld` files to view the logic or run the integrated simulation.

---

