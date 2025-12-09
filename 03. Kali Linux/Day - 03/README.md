<h1 align="center">💻 Day 3 🔄</h1>
<h2 align="center">📁 Linux File System 📁</h2>

---
### Linux File System
In Linux, the entire storage structure is organized like a single tree, with the root (/) at the top.

- **Everything is a file –** Devices, processes, sockets, and directories are represented as files.
> - The hierarchy **starts at / (root) and branches downward.**

- **Paths may be:**
  
  > - **Absolute Path :** begins with / (e.g., /home/Raj/Documents)
  > - **Relative Path :** starts from current directory (e.g., ../Downloads)

- [ ] **pwd –** Print Working Directory **(Shows your current absolute path.)**

#### Useful Path Shortcuts

|  cmd  |           Works           |
|-------|---------------------------|
|   .   |	Current directory         |
|  ..	  | Parent directory          |
|   ~	  | User’s home directory     |
|   /	  | Root directory            |

#### List Contents - ls

|    cmd    |           Works           |
|-----------|---------------------------|
|  ls       |  Basic listing            |
|  ls -a    |  Include hidden files     |
|  ls -lh   |  Human-readable sizes     | 
|  ls -ltr  |  Sort by modification time (oldest → newest) |


#### Change Directory - cd 

|    cmd    |           Works           |
|-----------|---------------------------|
|  cd /etc  |   Go to /etc              |
|  cd ..    |   Up one level            |
|  cd ~     |   To your home            |
|  cd -     | Back to previous location |

### Creating and Managing Directories

#### Make Directory - mkdir

 - mkdir Directory_name
 - mkdir -p Projects/2025/January
   
   > - **-p creates intermediate directories automatically.**

#### Remove Files or Directories

rmdir – Remove Empty Directories
rmdir OldFolder
 Works only if the directory is empty.
________________________________________
rm – Remove Files or Directories
rm file.txt
rm -r folder/        # remove directory recursively
rm -f file.txt       # force delete (no prompt)
rm -rf /test         # recursive + force
 Be careful with rm -rf / – it will erase everything.


