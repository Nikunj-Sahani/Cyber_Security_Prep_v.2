<h1 align="center">💻 Day 3 🔄</h1>
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

> - find /var/log -size +50M
> - find . -mtime -7

- **locate – Search Using Database**

 > - sudo updatedb
>  - locate shadow



