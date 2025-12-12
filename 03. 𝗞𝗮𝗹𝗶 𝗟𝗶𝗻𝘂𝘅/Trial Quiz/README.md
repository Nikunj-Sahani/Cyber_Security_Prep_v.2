<h1 align="center">🧑‍💻 KALI LINUX QUIZ's🧑‍💻</h1>

---
## Day - 01

#### 1. What is the core part of Linux responsible for managing hardware?
#### 2. Which command shows your current directory?
#### 3. What is the difference between /bin and /sbin?
#### 4. Which key combination opens a new terminal window?
#### 5. How do you view the manual of the ls command?

### ✈️ Tasks to do in Kali Linux Terminal : 
Run Commands and check it.
1. Display your username and working directory
2. Create a folder Practice and navigate into it in a line.
3. Create a new file named info.txt
4. Add text and view in info.txt
5. Copy and rename files
6. Remove the renamed file

---
## Day - 02

#### 1.	What does ls -l display?
#### 2.	Difference between rm and rmdir?
#### 3.	How to view the last 20 lines of a log file?
#### 4.	Which command changes file ownership?
#### 5.	How to find all .sh files modified in last 2 days?

### ✈️ Tasks to do in Kali Linux Terminal : 
Run Commands and check it.

1.	Create /home/student/practice
2.	Inside it, create file1, file2, file3
3.	Combine them → cat file1 file2 file3 > final.txt
4.	Copy final.txt to /tmp/backup/
5.	Compress it → tar -czvf backup.tar.gz /tmp/backup/
6.	Change permissions to execute only for owner → chmod 700 backup.tar.gz
7.	Remove temporary directory after verification.

---
## Day - 03

#### 1.	What’s the difference between chmod 755 and chmod 700?
#### 2.	How do you set file ownership to root:admins?
#### 3.	What is the effect of a sticky bit on /tmp?
#### 4.	Which file defines sudo permissions?
#### 5.	How do you list ACL permissions of a file?

### ✈️ Tasks to do in Kali Linux Terminal : 
Run Commands and check it.

1.	Create user student1 and group students
2.	sudo useradd -m student1
3.	sudo groupadd students
4.	sudo usermod -aG students student1
5.	Create shared folder /data/students
6.	sudo mkdir -p /data/students
7.	sudo chown root:students /data/students
8.	sudo chmod 2770 /data/students

---
## Day - 04

#### 1.	Which command shows real-time CPU and memory usage?
#### 2.	What is the difference between ps aux and top?
#### 3.	How do you stop a process running in the background?
#### 4.	Which command checks active services?
#### 5.	How do you schedule a command to run daily at 2 AM?

### ✈️ Tasks to do in Kali Linux Terminal : 
Run Commands and check it.

1.	Launch 3 background processes:
2.	ping google.com > pinglog &
3.	sleep 1000 &
4.	yes > /dev/null &
5.	Display all running processes:
6.	ps aux | less
7.	Check top resource consumers:
8.	top
9.	Kill one process:
10.	kill <PID>
11.	Schedule a reboot in 10 minutes:
12.	sudo shutdown -r +10 "System maintenance reboot"
13.	View logs for system boot:
14.	journalctl -b

---
## Day - 05

