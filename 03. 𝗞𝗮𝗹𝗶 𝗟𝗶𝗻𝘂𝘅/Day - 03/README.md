<h1 align="center">📒 Day 03 📒</h1>
<h2 align="center">📁 Linux File System 📁</h2>

---
### 👉 Linux File System
In Linux, the entire storage structure is organized like a single tree, with the root (/) at the top.

- **Everything is a file –** Devices, processes, sockets, and directories are represented as files.
> - The hierarchy **starts at / (root) and branches downward.**

- **Paths may be:**
  
  > - **Absolute Path :** begins with / (e.g., /home/Raj/Documents)
  > - **Relative Path :** starts from current directory (e.g., ../Downloads)

- [ ] **pwd –** Print Working Directory **(Shows your current absolute path.)**

#### 🖊️ Useful Path Shortcuts

|  cmd  |           Works           |
|-------|---------------------------|
|   .   |	Current directory         |
|  ..	  | Parent directory          |
|   ~	  | User’s home directory     |
|   /	  | Root directory            |

#### 🖊️ List Contents - ls

|    cmd    |           Works           |
|-----------|---------------------------|
|  ls       |  Basic listing            |
|  ls -a    |  Include hidden files     |
|  ls -lh   |  Human-readable sizes     | 
|  ls -ltr  |  Sort by modification time (oldest → newest) |


#### 🖊️ Change Directory - cd 

|    cmd    |           Works           |
|-----------|---------------------------|
|  cd /etc  |   Go to /etc              |
|  cd ..    |   Up one level            |
|  cd ~     |   To your home            |
|  cd -     | Back to previous location |

---
### 👉 Creating and Managing Directories

#### 🖊️ Make Directory - mkdir

 - mkdir Directory_name
 - mkdir -p Projects/2025/January
   
   > - **-p creates intermediate directories automatically.**

#### 🖊️ Remove Files or Directories

- **rm – Remove Files or Directories**

 > - **rm file.txt**    -----      # Normal Delete
 > - **rm -r folder/**      ----  # remove directory recursively
 > - **rm -f file.txt**    ----   # force delete (no prompt)
 > - **rm -rf /test**      ----   # recursive + force
 
- [ ] Note :- **Be careful with rm -rf/⭐ – it will erase everything.( means it Delete your Kali System)**

- **rmdir – Remove Empty Directories**

   > - rmdir directory_name - *Works only if the directory is empty.*
  
---
### 👉 File Creation and Manipulation

#### 🖊️ Create Files or Copy or Move

|  cmd   |           Works          |    Total cmd   |
|--------|--------------------------|----------------|
| touch  | To create text file      | **touch file.txt**  |
|  cp    | Copy Files and Folders   | **cp folder_name** |
| cp n n1 | Copy content of new → create new1 | **cp new.txt new1.txt** |
|  cp -r | Copy the entire directory | **cp -r source/ destination/**  |
|    mv  | Rename the file      |  **mv file new_name**  |
|  mv destination    |Move a file to another directory | **mv report.docx ~/Documents/**  |

> - **If need - Options: -v (verbose), -i (confirm overwrite).**

 #### 🖊️ Viewing File Content

| **Command** | **Description**                          | **Example**             |
| ----------- | ---------------------------------------- | ----------------------- |
|  cat        | Display entire file                      | **cat file.txt**        |
|  tac        | Display file backwards (last line first) | **tac log.txt**         |
|  head       | Show first 10 lines (default)            | **head -n 20 file.txt** |
|  tail       | Show last 10 lines                       | **tail -n 20 file.txt** |
|  less       | View file page by page, scrollable       | **less /etc/passwd**    |
|  nl         | Number each line of the file             | **nl script.sh**        |
|  wc         | Count lines, words, bytes                | **wc -lw file.txt**     |

#### 🖊️ Searching and Filtering Text

- **Search Patterns - grep**

 > - grep "root" /etc/passwd
 > - grep -rin "error" /var/log/

- **Options:**

  > - **-r** recursive
  > - **-i** ignore case
  > - **-n** show line numbers
  > - **-v** invert match

- **Search Files by Criteria - find**

> - find /home -type f -name "*.sh" 2> /dev/null - **Search in /home for all files (-type f) whose name ends with .sh**
> - find /home -type f –size +50M  2> /dev/null - **Search for files in /home that are larger than 50 MB**
> - find /home –type f –perm u=w 2>/dev/null - **ind files in /home where the user (owner) has write permission.**

- [ ] Note - **(ignore errors by redirecting them to /dev/null).**

> - find /var/log -size +50M - *Search inside /var/log for files larger than 50 MB.*
> - find . -mtime -7 - *Find files in current directory (.) that were modified within the last 7 days.*

- **locate – Search Using Database**

 > - sudo updatedb - **Updates the locate database**
 > - locate shadow - **/etc/shadow (where encrypted passwords are stored)**

---
### 👉 Archiving and Compression

| **Tool**        | **Create**                   | **Extract**                       | **Notes**                              |
| --------------- | ---------------------------- | --------------------------------- | -------------------------------------- |
| **tar**         | tar -cvf backup.tar dir/     | `tar -xvf backup.tar`             | *Creates archives only (no compression)* |
| **gzip**        | gzip file                    | `gunzip file.gz`                  | *Compresses **single files** only*       |
| **tar + gzip**  | tar -czvf backup.tar.gz dir/ | `tar -xzvf backup.tar.gz`         | *Most common compressed archive format*  |
| **zip / unzip** | zip -r archive.zip dir/      | `unzip archive.zip`               | *Windows-friendly, widely used*          |
| **bzip2 / xz**  | bzip2 file xz file         | `bunzip2 file.bz2` `unxz file.xz` | *High compression ratios (but slower)*   |

---
### 👉 Permissions and Ownership Basics
Each file has three sets of permissions:

- **Owner (u), Group (g), Others (o) —** *each with Read (r), Write (w), Execute (x).*

#### 🖊️ To check file or folder permission.
  > - **ls -l**

#### 🖊️ To give permission to file
- chmod 755 file_name
- chmod u+x file.sh

#### 🖊️ How the Permission value Works
- ✔️ **1st method by Numerical**
  
| Permission	| Value | Sign |
|-------------|-------|------|
|    Read	    |   4   |   r  |
|    Write    | 	2   |   w  |
|   Execute   |  	1   |   x  |

- **Example -** *chmod 754 file,* You have to add the value to give permission.
     > - **Owner (rwx) = 7**
     > - **Group (r-x) = 5**
     > - **Others (r--) = 4**

- ✔️ **2nd method by Letters**

|   Owner	  |  Sign |  Permissions |
|-----------|-------|--------------|
|   User	  | **u** |  Read ( r )  |
|   Group   | **g** |  Write ( w )  |
|   Others  | **o** | Execute ( x ) |

- **Example -**

  > - chmod u+r file_name **- give read(r) permission to user(u)**
  > - chmod g+w file_name **- give write(w) permission to group(g)**
  > - chmod o+rwx file_name **- give read, write, execute to others(o)**

#### 🖊️ To change owner or group of file
- chown owner_name file_name
- chgrp group_name file_name

#### 🖊️ To change both user or group in a command
- chown user:group file.txt
- chown -R user:group directory_name – **change ownership recursively**
---
### 👉 File Ownership and Access Control
To create a new user and managing.

- 🖊️ **Create and manage users**

|  command	|     Works    |
|-----------|--------------|
|  useradd  | To add user  |
|  userdel  | To delete user  |
|  passwd   | to set password |

**Example :-**
 > - sudo useradd <username> **- Add a new user.**
 > - sudo userdel <username>  **- Delete a user.**
 > - sudo passwd <username>  **- Set password for user.**

- 🖊️ **Show group membership**  

  > - groups <username> **- See groups of a user.**
  > - id <username>  **- See user ID + group ID + groups**

- [ ] **sudoers –** /etc/sudoers defines admin access.

---
### 👉 System Information Commands
🖥 System Information & Monitoring Commands (Linux)

|   Command   |       Function                             |   Example                        |
| ----------- | ------------------------------------------ | -------------------------------- |
| **uname -a**    | **Show full kernel & system info**             | `uname -r` (kernel version only) |
| hostnamectl | View or set hostname                       | `hostnamectl set-hostname lab1`  |
| **uptime**      | **Show system running time & load average**    | `uptime`                         |
| df -h       | Disk usage per filesystem (human readable) | `df -h /`                        |
| du -sh *    | Show folder sizes in current directory     | `du -sh /var/*`                  |
| free -h     | Show memory & swap usage                   | `free -h`                        |
| **top / htop**  | **Real-time process monitoring**               | `htop`                           |


### 👉 Networking Essentials

> - ping -c 4 google.com - **To check network is working.**
> - ip addr show - **To check IP address**

- netstat → shows network connections
- **netstat -anp | grep ssh**
  
   > - **-a →** show all ports
   > - **-n →** show port numbers (don’t convert names)
   > - **-p →** show which process is using the port
   > - **grep ssh →** filter the output and show only lines that contain ssh

---
### 👉 Redirection and Pipes (Linux)

| **Symbol** | **Meaning**                      | **Example**               |
| ---------- | -------------------------------- | ------------------------- |
| `>`        | Redirect output (overwrite file) | **`ls > list.txt`**           |
| `>>`       | Append output to file            | **`echo "end" >> file.txt`**  |
| `<`        | Take input from file             | **`sort < names.txt`**        |
| `Pipe Symbol`  | Pipe output to another command | `ls pipe symbol grep txt`          |

---
### 👉 Quick Cheat Sheet

|      Command          |       Function                          |
| --------------------- | --------------------------------------- |
| **ls -a**             |  List hidden files	                    |
| **file filename**     |  Show file type	                        |
|  **wc -l filename**   |  Count lines in file                    |
|  **diff file1 file2** |  Compare two files                      |
|  **ln file1 file2**   |   Create hard link                      |
|  **ln -s file1 linkname** |  Create symbolic link               |
|  **ls -l**                |  View permissions                   |
|  **df -h**                |  Check disk usage                   |
|  **grep "ERROR" /var/log/syslog** |  Search pattern in logs     |

---
### 🔄 Hands-On Lab – File Management

1.	Create /home/student/practice
2.	Inside it, create file1, file2, file3
3.	Combine them → cat file1 file2 file3 > final.txt
4.	Copy final.txt to /tmp/backup/
5.	Compress it → tar -czvf backup.tar.gz /tmp/backup/
6.	Change permissions to execute only for owner → chmod 700 backup.tar.gz
7.	Remove temporary directory after verification.

### 🔄 Pro Tips
- Use alias for frequent commands → alias ll='ls -lAh'
- Press Tab to auto-complete paths
- Use Ctrl + R to search command history
- Use sudo !! to rerun last command as root
- Avoid using root account directly—use sudo

### ✅ Quiz – Chapter 2
1.	What does ls -l display?
2.	Difference between rm and rmdir?
3.	How to view the last 20 lines of a log file?
4.	Which command changes file ownership?
5.	How to find all .sh files modified in last 2 days?

---
