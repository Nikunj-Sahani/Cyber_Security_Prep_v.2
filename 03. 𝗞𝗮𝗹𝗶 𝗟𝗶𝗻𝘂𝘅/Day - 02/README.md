<h1 align="center">📒 Day 02 📒</h1>
<h2 align="center">🧑‍💻 KALI LINUX INTRODUCTION 🧑‍💻</h2>

---
## What is Linux?
Linux is a free and open-source operating system based on UNIX. It **controls hardware** and provides a platform to run software.

### ⭐ Key Features of Linux

> - **Open Source	-** Free to use and modify (licensed under **GPL – GNU General Public License**)
> - **Secure -**	Strong permission, firewall & SELinux
> - **Stability -** 	Rare crashes, long-term servers run
> - **Multi-User -**	Multiple users at same time
> - **Multi-Tasking -**	Run many apps together
> - **Portable -**	Runs on PCs, mobiles, servers, IoT
> - **Customizable	-** You can modify OS as per needs

### Where linux mostly Used 
Used by developers, system administrators, ethical hackers, and cybersecurity professionals.
 - [ ] Servers & Data Centers
 - [ ] Cybersecurity & Ethical Hacking
 - [ ] Cloud & DevOps
 - [ ] IoT & Embedded Devices and SuperComputers

### 🔧 Main Components of Linux
Linux OS is mainly divided into **5 components:**

- **System Utilities & Applications** ⏩ *Tools to control system and run tasks* Example: cp, mkdir, text editors, browsers, servers.
- **Shell** ⏩ *Command interpreter* (user interacts with OS or kernal), Example: Bash, Zsh
- **Kernel** ⏩ *Core of Linux*:- controls all hardware and manages system resources.
- **Hardware** ⏩ *Physical components* (CPU, RAM, Disk, Network Interface).
- **File System** ⏩ Organizes data in directories/files , Example: ext4, xfs

---
### ✔ Linux Distributions
Different companies and communities build custom versions of Linux called distributions.

|  Distribution  |    Based On    |          Common Use          |
|----------------|----------------|------------------------------|
|   **Ubuntu**	  |    **Debian**  |	**User-friendly desktop/server** |
|     Debian	    |    Original    |	Stable & secure              |
|     Fedora     |    	Red Hat    |	Developer focus              |
|CentOS/AlmaLinux|   	Red Hat	    | Enterprise servers           |
|   Arch Linux   |   Independent  |	Custom & advanced users      |
| **Kali Linux**	|   **Debian**   |	**Cybersecurity & penetration testing** |
|  **Parrot OS** |  	**Debian**   |	**Ethical hacking & digital forensics** |

### ✔ Unix Structure
<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/03.%20Kali%20Linux/Images/Linux.png" alt="Sample Image" width="800" height="1000"></div>

---
## 🎪 Kali Linux 🎪
---
### ⚓ Shell
The shell is the command interpreter that **takes input and executes it.**
It communicates between user and kernel.

> - 📌 **Default Shell in Kali Linux → Zsh (Z Shell)**
> - (*Previously Bash was the default shell*)

### ⚓ Terminal
A terminal is a CLI environment (Command Line Interface). It allows users to *run commands and interact with the OS.*

> - 📌 In Kali Linux → Default Terminal is **GNOME Terminal** (or XTerm in other desktops).

---
- 🎈 **Terminal :-**	Window that displays input/output.
- 🎈 **Shell :-**	Interpreter that executes commands.

#### Shortcut to Open Terminal
 - [ ] Ctrl + Alt + T (on Desktop)
 - [ ] Ctrl + Alt + F2 (Through a TTY - TeleType Terminal).
       
   > - 🧠 **What is TTY?**
   > - It is a text-only virtual console
   > - Works without GUI (no Desktop environment needed

### 🐧 Common Shells in Kali Linux:

| Shell | 	  Description   |
|-------|-------------------|
|  **Zsh**  |	**Default in Kali**, advanced and customizable |
| Bash	 | **(Bourne Again Shell)**, Most common Linux shell, widely used |
| Fish	 | User-friendly with auto-suggestions |
|  Sh   |	Basic shell (Bourne shell) |

---
## 🎏 Linux Command Syntax
Every Linux command generally follows this structure:
  - [ ] **command  [options]  [arguments]**

   > - **command -** The action you want to perform.
   > - **options -** Modify how the command works.
   > - **arguments -** The file, directory, or target to apply the action on.

- Example: **ls -l /home**
  
  > - **ls →** Command
  > - **-l →** Option (long listing format)
  > - **/home →** Argument (target directory)

## 🎏 Basic Linux Commands

### 📂 File & Directory Commands

| Command                  | Description                     |
| ------------------------ | ------------------------------- |
| **`ls`**                 | **List files in current directory** |
| `ls -la`                 | List all files with details     |
| `pwd`                    | Show current working directory  |
| **`cd foldername`**      | **Change directory**                |
| `cd ..`                  | Go back to previous directory   |
| **`mkdir folder`**       | **Create a new folder**             |
| `rmdir folder`           | Remove empty folder             |
| **`rm file`**            | **Delete file**                     |
| `rm -r folder`           | Delete folder with content      |
| **`cp source dest`**     | **Copy file/folder**                |
| `mv source dest`         | Move/rename file/folder         |
| `touch file.txt`         | Create empty file               |
| **`cat file.txt`**       | **View file content**               |
| **`nano file.txt`**      | **Open file in nano editor**        |
| `echo "text" > file.txt` | Create file with text           |
| **`clear`**              | **Clears the terminal screen**     |
| `man`                    |	Displays command manual        |
| `history`	               | Shows command history          |	
| **`exit`**	              | **Closes the shell**	              |
| `echo`	( echo $USER )    | Prints message or variable	    |

#### **Copy, Move, Rename:**
  
  > - cp file1.txt ~/tmp/ ::- **(Copy file and pasting in tmp folder).**
  > - mv file1.txt file2.txt ::- **( Renaming the file name).**
  > - mv file.txt ~/path/ ::- **(Move file to folder path)**


### 🌐 Networking Commands

| Command                 | Description              |
| ------------------------| ------------------------ |
| **`ifconfig` / `ip a`** | **Show IP address**          |
| **`ping website.com`**  | **Test connectivity**        |
| `netstat -tulnp`    | Show open ports          |
| `curl URL`          | Download webpage         |
| `ssh user@ip`       | Connect to remote system |

### 🧠 System Information

| Command    | Description         |
| ---------- | ------------------- |
| `uname -a` | System info         |
| `hostname` | Show system name    |
| `df -h`    | Disk usage          |
| `free -h`  | Memory usage        |
| `top`      | Active processes    |
| `uptime`   | System running time |
| `date`     | Show date & time    |

### 👤 User & Permission Commands

| Command                 | Description              |
| ----------------------- | ------------------------ |
| **`whoami`**            | **Show current user**    |
| `id`                    | User + group information |
| **`chmod 755 file`**    | **Change file permission**  |
| `chown user:group file` | Change ownership         |
| **`passwd`**            | **Change user password** |

### 📦 Package Management (Debian/Kali/Ubuntu)

| Command                    | Description          |
| -------------------------- | -------------------- |
| **`sudo apt update`**          | Update package lists |
| **`sudo apt upgrade`**         | Install new updates  |
| **`sudo apt install pkgname`** | Install software     |
| `sudo apt remove pkgname`  | Remove software      |

---
## 🗂️ Linux File System Hierarchy
📌 Everything in Linux starts from the root directory /. All files, folders, devices → inside / (slace)

| Directory | Full Name           | Purpose                                  |
| --------- | ------------------- | ---------------------------------------- |
| `/`       | Root                | Top of file system (starting point)      |
| **`/home`**   | **Home Directory**      | **Personal files of users**                  |
| **`/root`**   | **Root User’s Home**    | **Superuser’s private folder**               |
| `/bin`    | Binary              | Basic commands (ls, cp, mv, cat)         |
| `/sbin`   | System Binary       | System admin commands (ifconfig, reboot) |
| **`/etc`**    | **Configuration Files** | System config files, network, services   |
| **`/var`**    | **Variable Files**      | **Logs, spool files, cache**                 |
| `/usr`    | User Programs       | Installed software, libraries            |
| `/tmp`    | Temporary           | Temporary files (auto delete)            |
| **`/lib`**    | **Libraries**           | **Shared libraries for system**              |
| `/dev`    | Devices             | Hardware as files (USB, HDD, etc.)       |
| `/media`  | Removable Media     | Auto mount USB/CD                        |
| `/mnt`    | Mount               | Manual mount point for drives            |
| `/opt`    | Optional            | Optional or 3rd party software           |
| **`/boot`**   | **Boot Files**          | **GRUB, kernel for system startup**          |
| `/proc`   | Process Files       | Virtual directory – system processes     |
| **`/sys`**    | **System Info**         | **Hardware & kernel info**                   |

### 🧠 Quick Memory Tricks:

- **/home =** Users' personal files
- **/etc =** All system configurations
- **/bin + /sbin =** Commands
- **/root =** Admin’s private home
- **/var/log =** Very important logs
- **/tmp =** Temporary workspace

#### 📌 Example Path:
- [ ] **/home/user/Documents/file.txt**
      
  > - / root → system start
  > - /home → user directory
  > - /user → account name
  > - /Documents → user folder
  > - file.txt → file

---
# Practice : Basic Commands
Explore Linux shell, file structure, and commands.
- **Tasks to do in Kali Linux Terminal :** Run Commands and check it.

> - **1.**	Display your username and working directory
> - **2.**	Create a folder Practice and navigate into it in a line.
> - **3.**	Create a new file named info.txt
> - **4.**	Add text and view in info.txt
> - **5.**	Copy and rename files
> - **6.**	Remove the renamed file

## Important Tips for Beginners
 - Use **Tab** for auto-completion
 - Use **↑ / ↓** arrows to navigate previous commands
 - Use **Ctrl + C** to stop a running process
 - Use **Ctrl + D** to log out or end input
 - Explore **man** pages often

### 🧠 Linux Basics Quiz
#### ✔ Multiple Choice Questions (MCQ)

1️⃣ **Linux kernel was first developed by:**
- A) Bill Gates
- B) Linus Torvalds
- C) Dennis Ritchie
- D) Richard Stallman

2️⃣ **The default shell in Kali Linux is:**
- A) Bash
- B) Zsh
- C) Fish
- D) Sh

3️⃣ **Which directory contains user personal files?**
- A) /etc
- B) /home
- C) /bin
- D) /var

4️⃣ **Which command shows current working directory?**
- A) ls
- B) pwd
- C) cd
- D) home

5️⃣ **/bin directory stores:**
- A) Log files
- B) Device files
- C) Basic system commands
- D) User directories

6️⃣ **To see network IP configuration:**
- A) ip a
- B) ls
- C) mkdir
- D) uname

7️⃣ **rm -r foldername does what?**
- A) Remove only empty directory
- B) Remove directory with all contents
- C) Rename directory
- D) Create directory

8️⃣ **Ctrl + Alt + F2 opens:**
- A) BIOS settings
- B) Terminal GUI
- C) TTY (Text-mode terminal)
- D) File Explorer

9️⃣ **Which directory stores boot loader files?**
- A) /boot
- B) /var
- C) /usr
- D) /dev

🔟 **Which command shows manual/help pages?**
- A) help
- B) info
- C) man
- D) doc

#### ✍ Short Questions (Try to answer yourself)

- [ ] What is the difference between Shell and Terminal?
- [ ] Write the Linux command syntax format.
- [ ] What is the role of /etc directory?
- [ ] What does cd .. do?
- [ ] Expand: TTY

#### ☑ BONUS (If you want extra challenge)
Write commands for:

- [ ] Create a folder named test
- [ ] Create a file inside it named notes.txt
- [ ] Display content of the file
- [ ] Delete folder along with file

---
---
