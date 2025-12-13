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
### Understanding File Ownership




