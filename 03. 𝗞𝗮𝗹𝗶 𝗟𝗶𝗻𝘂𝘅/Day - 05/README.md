<h1 align="center">📒 Day 05 📒</h1>
<h2 align="center">🛒 Process & System Management 🛒</h2>

---
## 🎗️ Understanding Processes in Linux
A process is a running instance of a program.
 > - **When you execute a command, Linux creates a process with a unique PID (Process ID).**

### 🎮 Linux Process States

| **State**                 | **Symbol** | **Meaning**                                              |
| ------------------------- | ---------- | -------------------------------------------------------- |
| **Running**               | R          | Process is actively running or ready to run              |
| **Sleeping**              | S          | Waiting for an event or resource (interruptible)         |
| **Uninterruptible Sleep** | D          | Waiting for I/O, cannot be killed                        |
| **Stopped**               | T          | Process stopped, usually by a signal (e.g., Ctrl+Z)      |
| **Zombie**                | Z          | Process finished but still has an entry in process table |
| **Tracing/Debugging**     | t          | Being traced or debugged by another process              |

### 🎮 Viewing Processes - Screenshot
Quick command to see process states: **ps**

  > - **ps**  ----- # Show current shell processes
  > - **ps aux** ----- # Show all processes with details
  > - **ps -ef**  -----# Full-format listing (alternative view)

- 📱 **Common Columns:**

   > - USER → Process owner
   > - PID → Process ID
   > - %CPU / %MEM → Resource usage
   > - STAT → Process stat

addding picture

### 🎮 Real-time Process Viewing
Quick command to see process states: **top**

- *Press buttons to sort by view:*
  > - P → Sort by CPU
  > - M → Sort by memory
  > - k → Kill a process
  > -  q → Quit

adding pic 

- 📱 **Enhanced Process Viewer : htop**
  > - sudo apt install htop
  > - **htop**
  > - View mode in - Color-coded, interactive, and more readable than top.

adding pic 

---
### 📶 Monitoring System Resources

| **Command** | **Purpose**                | **Example**       |
| ----------- | -------------------------- | ----------------- |
| `uptime`    | Show system load averages  | `uptime`          |
| `vmstat 5`  | Monitor memory, CPU, swap  | `vmstat 5`        |
| `iostat`    | Disk I/O statistics        | `iostat -xz 5`    |
| `free -h`   | Show memory usage          | `free -h`         |
| `df -h`     | Disk usage per mount point | `df -h`           |
| `du -sh *`  | Show directory sizes       | `du -sh /var/*`   |
| `mpstat`    | CPU usage per core         | `mpstat -P ALL 5` |

---
## 🎗️ Managing Processes
