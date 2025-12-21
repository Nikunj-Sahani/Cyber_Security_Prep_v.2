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

- ❌ **Kill or Stop a Process**

| **Command**         | **Purpose**                     | **Example**       |
| ------------------- | ------------------------------- | ----------------- |
| `kill <PID>`        | Graceful stop (SIGTERM)         | `kill 1234`       |
| `kill -9 <PID>`     | Force kill (SIGKILL)            | `kill -9 1234`    |
| `killall <process>` | Kill all instances of a process | `killall firefox` |

   > - **Use kill first to stop the process.**
   > - **-9 only if the process doesn’t stop.**

- 📵 **Set Process Priority - nice & renice**

   > - nice -n 10 command  -----  # **Start with lower priority**
   > - renice 5 -p 1234  -------   # **Change existing process priority**

- 🔄 **Background and Foreground - bg / fg**

| **Command**    | **Purpose**                | **Example**    |
| -------------- | -------------------------- | -------------- |
| `sleep 1000 &` | Run command in background  | `sleep 1000 &` |
| `jobs`         | List background jobs       | `jobs`         |
| `fg %1`        | Bring job 1 to foreground  | `fg %1`        |
| `bg %1`        | Resume job 1 in background | `bg %1`        |

---
### 🔐 nohup – Run Process Immune to Logout

| **Command** | **Purpose**                             | **Example**                 |
| ----------- | --------------------------------------- | --------------------------- |
| `nohup`     | Run process that continues after logout | `nohup python3 script.py &` |

   > - 👉 **Output is saved to nohup.out by default.**

- 🎄 **Process Tree and Parent Relationships**

   > - pstree – Display Process Hierarchy
   > - **pstree -p :-** Shows parent/child relationships (e.g., services spawned by systemd).

---
### 🎏 System Services and Daemons

-  **🔄 Control systemd Services - systemctl**

   - [ ] sudo systemctl status ssh
   - [ ] sudo systemctl start nginx
   - [ ] sudo systemctl stop apache2
   - [ ] sudo systemctl restart ssh
   - [ ] sudo systemctl enable nginx
   - [ ] sudo systemctl disable apache2

| **Command**        | **Description**                   |
| ------------------ | --------------------------------- |
| `status`           | Show current service status       |
| `start / stop`     | Start or stop a service           |
| `restart`          | Restart a service                 |
| `enable / disable` | Enable or disable service at boot |

  > - **systemctl list-units --type=service :-** List all active services.

### 🎏 System Startup and Shutdown

| **Command**                   | **Purpose**                     |
| ----------------------------- | ------------------------------- |
| `sudo shutdown now`           | Power off immediately           |
| `sudo shutdown -r now`        | Reboot immediately              |
| `sudo poweroff`               | Power off system                |
| `sudo reboot`                 | Restart system                  |
| `sudo shutdown +15 "message"` | Schedule shutdown in 15 minutes |
| `sudo shutdown -c`            | Cancel scheduled shutdown       |

  > - **Scheduled shutdown sends a warning message to logged-in users.**

---
### 🎏 System Logging and Monitoring
Logs are critical for troubleshooting and auditing. **Linux stores logs mainly under /var/log/.**

- 📄 **Important Linux Log Files**
  
| **Log File**        | **Description**             |
| ------------------- | --------------------------- |
| `/var/log/syslog`   | General system messages     |
| `/var/log/auth.log` | Login & authentication logs |
| `/var/log/dmesg`    | Kernel ring buffer messages |
| `/var/log/boot.log` | System boot information     |
| `/var/log/cron`     | Cron job activity           |

- **Kernel Messages ; -** dmesg | less

- 📄 **View systemd  logs**

  > - sudo journalctl ---------- **# View systemd logs**
  > - sudo journalctl -u ssh.service ------ **# View logs for a service**
  > - sudo journalctl --since "1 hour ago"  ------ **# View logs since a time**

---
### 🎏 Task Scheduling (Automation)

- ⏰ **Schedule Repetitive Tasks - Cron**

| **Command**  | **Purpose**          |
| ------------ | -------------------- |
| `crontab -e` | Edit cron jobs       |
| `crontab -l` | View cron jobs       |
| `crontab -r` | Remove all cron jobs |

- [ ] **Cron Job Example**
  
   > - **0 2 * * * /usr/bin/rsync -av /home /backup/**
   > - 👉 Runs daily at 2 AM

- ⏰ **Cron Time Fields**

| **Field**    | **Meaning** | **Values**              |
| ------------ | ----------- | ----------------------- |
| Minute       | Minute      | `0–59`                  |
| Hour         | Hour        | `0–23`                  |
| Date of Month| Day         | `1–31`                  |
| Month Name   | Month       | `1–12`                  |
| Day of Week  | Weekday     | `0–7` (Sunday = 0 or 7) |

   > - **crontab -l** --- View cron jobs
   > - **crontab -r** --- Remove cron jobs

### ⏰ Schedule One-Time Tasks - at

| **Command** | **Purpose**              |
| ----------- | ------------------------ |
| `at 10:30`  | Schedule a task at 10:30 |
| `Ctrl + D`  | Save and exit            |

- 👉 **Manage at Jobs :-** List or remove scheduled jobs:

| **Command**    | **Purpose**            |
| -------------- | ---------------------- |
| `atq`          | List scheduled jobs    |
| `atrm <jobid>` | Remove a scheduled job |

---
### 🖥️ System Information and Diagnostics

> - **hostnamectl :-**	View/Change hostname
> - **lsblk :----------**	List block devices
> - **lscpu :---------**	Display CPU information
> - **lsusb :---------**	List USB devices
> - **lspci :---------**	List PCI devices
> - **uptime :------**	Show system uptime
> - **who -a :------**	Show logged-in users
> - **w :------------**	Show active users
> - **sar :----------**	Performance monitoring (sysstat package)

### 🖥️ Memory and Disk Optimization

- **🔄 Free RAM Cache (Advanced)**
   > - sudo sync
   > - sudo sh -c 'echo 3 > /proc/sys/vm/drop_caches'

- **🔄 Swap Management**
   > - free -h
   > - sudo swapon -s
   > - sudo swapon /swapfile
   > - sudo swapoff /swapfile

- **🔄 Mount and Unmount Drives**
   > - sudo mount /dev/sdb1 /mnt
   > - sudo umount /mnt

---
---
## Hands-On Lab – System Monitoring & Process Control
Goal: Monitor, control, and automate Linux system performance.

- **Tasks to do:**

1.	Launch 3 background processes:
2.	ping google.com > pinglog &
3.	sleep 1000 &
4.	yes > /dev/null &
5.	Display all running processes:
6.	Check top resource consumers:
7.	Kill one process:
8.	Schedule a reboot in 10 minutes:
9.	View logs for system boot:
10.	Start a software with terminal.

## 🛠 Linux Troubleshooting Commands

| **Problem**         | **Solution**                 |
| ------------------- | ---------------------------- |
| Hung process        | `kill -9 <PID>`              |
| Unresponsive system | `dmesg`                      |
| Network issue       | `ping`, `ss`, `traceroute`   |
| Disk full           | `du -sh /*`, `df -h`         |
| Service failed      | `systemctl status <service>` |
| Check boot issues   | `journalctl -xe`             |

## Quiz

1.	Which command shows real-time CPU and memory usage?
2.	What is the difference between ps aux and top?
3.	How do you stop a process running in the background?
4.	Which command checks active services?
5.	How do you schedule a command to run daily at 2 AM?

---





