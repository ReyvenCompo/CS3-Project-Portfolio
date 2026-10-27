# WORKSHEET 1

## Observe and Analyze a Real-World Process

---

## 1. Project Information

| Information                | Details |
| -------------------------- | ------- |
| **Proposed Project Title** | CRAM-NET (Campus Resource Allocation for Academic Priority Network)   |
| **Team Members**           | 1.Alboroto Francis      |
|                            | 2.Asentista, Eden      |
|                            | 3.Compo, Reyven      |
|                            | 4.Duadua, Gillian      |
|                            | 5.Martinez, Romart      |
|                            | 6.Soguilon, Yno      |
| **PSHS-DRC Area/Location** | Acad Building 1        |

---

## 2. Observe the Current Process

### 1. What process did you observe?

> The process of campus-wide Wi-Fi connection, bandwidth access, and digital resource usage by students and school personnel inside the Acad 1 building during active class and study hours.

<br>

### 2. What is the purpose of this process?

> To provide stable internet connectivity across classrooms and study areas, enabling users to access educational portals, stream instructional media, submit academic requirements, and conduct research.

<br>

### 3. Who are involved in the process?

**(Up to two roles only.)**

| Person/Role | Responsibility in the Process |
| ----------- | ----------------------------- |
| 1. Students | Connect to the school Wi-Fi network to access online learning portals, download learning materials, and complete research or assignments.                             |
| 2. Teachers | Use the Wi-Fi network to access online educational content, stream lecture media, and manage digital classroom activities.                             |

### 4. What are the steps in the current process?

| Step | What happens? | Person/Role Involved |
| ---- | ------------- | -------------------- |
| 1    | Users enter their classroom of the academic building for classes or study sessions. |  Students & Teachers  |
| 2    | Users attempt to connect their devices to the school's free Wi-Fi network from their current location. | Students & Teachers |
| 3    | Signal quality varies depending on room location. |  Students & Teachers |
| 4    | Users far from the router experience severe bandwidth drops, frequent timeouts, and connection dropouts while accessing educational resources. | Students & Teachers |
| 5    | Affected users must physically relocate to high-coverage sections of the building, pause digital activities, or switch to offline work. | Students & Teachers |

---

## 3. Analyze the Problem

### 1. What problems or difficulties did you observe?

> The current Wi-Fi system treats all connected devices equally regardless of user role or task urgency. During peak hours, non-essential high-bandwidth consumption (such as video streaming or background updates) starves students who are trying to access learning portals or submit urgent academic requirements, causing slow loading times, network timeouts, and unfair bandwidth starvation in congested areas of Acad 1.

<br>

### 2. Which part of the process could be improved or automated?

> Steps 3 and 4 can be significantly improved by automating bandwidth allocation based on user role and task urgency. Instead of a static "first-come, first-served" connection model, a software-based dynamic bandwidth throttler can automatically detect high-priority academic tasks (e.g., student submissions and deadlines) and re-route higher network speeds to them in real time.

<br>

---

## 4. Propose a Simple Solution

### 1. What would your proposed system do?

> CRAM-NET is a software-based bandwidth allocation simulator that dynamically manages Wi-Fi speed distribution in Acad 1. It prioritizes students working on urgent academic tasks during study/class hours, shifting bandwidth allocation from lower-priority devices to ensure students complete their requirements without network delays.

<br>

### 2. Who would use the system?

| User/Role | Possible Use |
| --------- | ------------ |
| 1.Students        |Log into the system, select their current task urgency level (e.g., urgent submission, general research), and receive optimized bandwidth speed.              |
| 2.School Personnel / Administrators        |Monitor current network usage trends, view active session bandwidth queues, and adjust base speed limits for different user groups.              |

### 3. What are the essential features?

> **Keep your proposed system simple. Your project will be subject to teacher approval.**

| Feature | Purpose |
| ------- | ------- |
| 1.Workload-Based Role Login      |Classifies users as Student or Personnel and records active academic task urgency (e.g., ongoing research, impending assignment deadline) to set base network priority.| 
| 2.Dynamic Student-Centric Bandwidth Allocator      |Automatically shifts available bandwidth capacity to students during active academic hours and project deadlines, throttling lower-priority or background network traffic.| 
| 3.Automated Traffic & Activity Logger      |Logs session bandwidth consumption and generates a clear summary table flagging high-usage vs. academic traffic to keep the network optimized.| 

