<h1 align="center">💻 Day 04 🔄</h1>
<h2 align="center">🧑‍💻 USER AND PERMISSION MANAGEMENT 🧑‍💻</h2>

---
### 👤 Understanding Users and Groups
In Linux, every action is performed by a user — and every user belongs to one or more groups.

- A **User** is an account that can log in and use the system.
- A **Group** is a collection of users to manage permissions easily.
- A **Root** is Superuser with full system control.

|      Type       | Description                            |
| --------------- | -------------------------------------- |
| **Normal user** | Regular login user                     |
| **System user** | Used by services (UID < 1000)          |
| **Primary group**   | Default group of a user            |
| **Secondary group** | Additional groups for extra access |
| **UID**         | User ID (unique number for each user)  |
| **GID**        | Group ID (unique number for each group) |

### 📁 Important Files for Users and Groups
You can see all users and groups listed in this folders.

- [ ] /etc/passwd → **User information**
- [ ] /etc/group  → **Group information**
- [ ] /etc/shadow → **Encrypted passwords (readable only by root)**

 > - Note - For open this files, use **cat command**.

### 👤 Default System Users
System users are automatically created during Linux installation.

   - root :– *Administrative user*
   - daemon, bin, sys, mail :– *System service accounts*
   - nobody :– *Minimal permission user (used for guest or test processes)*

---
### ➕ User & Group Management Commands

| Task              | Command                      |
| ----------------- | ---------------------------- |
| Create user       | `useradd username`           |
| Delete user       | `userdel username`           |
| Create group      | `groupadd groupname`         |
| Add user to group | `usermod -aG group username` |
| Set/Change password   | `passwd username`        |
| Switch user       | `su - username`              |

- 🕹️ **Assign shell to user** 
   > - sudo chsh -s /bin/zsh username

- 🕹️ **Create User with Home Directory and Default Shell**
   > - sudo useradd -m -s /bin/bash username

     > - **-m :-** Create home directory
     > - **-s :-** Specify login shell
     > - **bash :-** Shell (like sh , zsh)

- 🕹️ **Modify User**
   > - sudo usermod -aG sudo username   →---------→    # Add user to sudo group
   > - sudo usermod -d /data username   →----------→   # Change home directory of username
   > - sudo usermod -l newname username  →------→  # Rename user

     > - **-aG :-** Append Group (Add to group)
     > - **-d :-** Directory
     > - **-l :-** Login to new name
  
- 🕹️ **Delete Userid**
  > - sudo userdel useranme          # Delete the user
  > - sudo userdel -r username             # Remove user + home directory

    > - **-r :-** Recursive (Delete all)

- 🕹️ **View Group Membership**
   > - groups username
   > - id username

- 🕹️ **Remove User from Group**
   > - sudo gpasswd -d username groupname
   > - sudo groupdel groupname --- **Delete Group**

     > - **gpasswd -** To delete user from group

---
### 📌 Understanding File Ownership
In Linux, every file and directory is owned by: **User & Group.** Ownership decides who can read, write, or execute the file.

- 🎲 **Each Linux file has 3 Things :-**

  > - **Owner (User)**
  > - **Group**
  > - **Permissions (rwx)**

- ♦️ *For Example:*
   > - **Create a file -** file.txt
   > - **Check permission -** ls -l file.txt
   
     > - **-rw-r-xr-- 1 username groupname 1024 Nov 13 12:15 file.txt**

- 🎲 **Understand Permission of file**

  > - rw-r-xr-- 1 username groupname 1024 Nov 13 12:15 file.txt

   > - ♦️ **Part of permission -**
   > - **rw- :-** owner (read , write)
   > - **r-x :-** group (read , execute)
   > - **r-- :-** others (read)
  
    > - username → **Owner**
    > - groupname → **Group**

---
### 🖥 File Permissions Explained
I'm explaining this again to more understand.

- 🖊️ **To check file or folder permission.**
  > - ls -l

- 🖊️ **To give permission to file**
   > - chmod 755 file_name = *Numerical Method*
   > - chmod u+x file.sh = *Character Method*

### 🖊️ How the Permission value Works
- ✔️ **1st method by Numerical**
  
| Permission	| Value | Sign |
|-------------|-------|------|
|    Read	    |   4   |   r  |
|    Write    |  	2   |   w  |
|   Execute   |  	1   |   x  |

- **Example -** You have to add the value to give permission.
 1.  > - *chmod 754 file,* 
     > - **Owner (rwx) = 7**
     > - **Group (r-x) = 5**
     > - **Others (r--) = 4**

 2.  > - *chmod 524 file.txt*
     > - **Owner (r-x) = 5**
     > - **Group (-w-) = 2**
     > - **Others (r--) = 4**
 
- ✔️ **2nd method by Letters**

|   Owner	  |  Sign |  Permissions |
|-----------|-------|--------------|
|   User	   | **u** |  Read ( r )  |
|   Group   | **g** |  Write ( w )  |
|   Others  | **o** | Execute ( x ) |
| u , g , o | **a** | a means all |

- **Example -**

  > - chmod u+r file_name **- give read(r) permission to user(u)**
  > - chmod g+w file_name **- give write(w) permission to group(g)**
  > - chmod o+rwx file_name **- give read, write, execute to others(o)**

  > - chmod a+rwx file_name **- give permission to all.**

---
### 📌 Changing Ownership and Groups
Change the owner of a file.

- 🖊️ **To change owner or group of file**
   > - chown owner_name file_name
   > - chgrp group_name file_name

- 🖊️ **To change both user or group in a command**
   > - chown user:group file.txt
   > - chown -R user:group directory_name – **change ownership recursively**

---
### ♟️ Special Permissions
Sometimes, standard rwx isn’t enough — we use **special bits.**

| **Type**                | **Symbol**    | **Purpose**                                                        |
| ----------------------- | ------------- | ------------------------------------------------------------------ |
| **SUID (Set User ID)**  | `s` on owner  | Execute file with **file owner’s privileges**                      |
| **SGID (Set Group ID)** | `s` on group  | Execute file with **group owner’s privileges**                     |
| **Sticky Bit**          | `t` on others | Protect shared directories (users can delete only their own files) |



