# Assignment - 2
## Shell Scripting

>Name: Aman Narnaware
>
>Roll: 322005
>
>Batch: B1
>
>PRN: 22110404

### 1. What is Shell (Linux kernel architecture diagram)
   
  In the context of Linux operating systems, a shell is a program that interprets commands. It provides the user interface for accessing the operating system's services. The shell acts as an intermediary between the user and the kernel (the core component of the operating system). When a user enters a command, the shell interprets it, executes it by calling the appropriate system programs, and then returns the results to the user.
```
+------------------------+ 
|         Shell          |      <-- Command interpreter and user interface 
+------------------------+ 
|   Application Programs |      <-- User-level programs 
+------------------------+ 
|   System Libraries     |      <-- Standard C libraries, etc. 
+------------------------+ 
|        Kernel          |      <-- Core of the operating system 
+------------------------+ 
|       Hardware         |      <-- Physical computer hardware 
+------------------------+ 
```
  The Linux kernel architecture diagram typically consists of several layers. At the lowest level is the hardware, followed by the kernel, which manages hardware resources and provides essential services. Above the kernel are various system libraries and utilities, including the shell. The shell interacts with the kernel through system calls to perform tasks such as process management, file manipulation, and input/output operations.

### 2. Different types of shells

In the Linux and Unix environments, there are several types of shells available, each with its own features and capabilities. Some of the most common types of shells include:

a. **Bourne Shell (sh):** Developed by Stephen Bourne at AT&T's Bell Labs, the Bourne Shell is one of the oldest Unix shells. It provides basic functionality for executing commands, scripting, and control flow structures like loops and conditionals.

b. **Bourne-Again Shell (bash):** Bash is the default shell for most Linux distributions. It is backward-compatible with the Bourne Shell but includes additional features such as command-line editing, history, and job control. Bash is highly customizable and widely used by both casual users and system administrators.

c. **C Shell (csh):** Developed by Bill Joy at the University of California, Berkeley, the C Shell features a C-like syntax and interactive command-line editing. It introduced several innovative features at the time, such as history substitution and aliases.

d. **Korn Shell (ksh):** Developed by David Korn at Bell Labs, the Korn Shell combines features from the Bourne Shell and the C Shell while introducing its own enhancements. It offers advanced scripting capabilities, command-line editing, and programmable completion.

e. **Z Shell (zsh):** Zsh is an extended Bourne Shell with additional features for interactive use and scripting. It includes powerful tab completion, spelling correction, and advanced customization options. Zsh is highly configurable and often preferred by power users.


### 2a) Write a shell script to check user is root user or not

```
#!/bin/bash

# Check if the user is root
if [ "$(id -u)" = "0" ]; then
    echo "You are the root user."
else
    echo "You are not the root user."
fi
```

**Output**

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/12108a44-151e-4f51-971f-470e29a8284e)

---

### 2b) Write a shell script to install any particular software (ex: java or python)

```
#!/bin/bash

sudo apt update

# Install Python (assuming apt package manager, use yum if any other linux distro)
sudo apt install python3
```

**Output**

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/616ac009-4eab-4ff0-96b4-d4b09bd192e9)

---

### 2c) Write a shell script to check disk usage of the system and if disk usage is more than 90% it should send an email to system admin. This script should run everyday at 8:00 AM.

```
#!/bin/bash

# Set threshold for disk usage (90%)
threshold=90

# Get disk usage percentage for the root filesystem
disk_usage=$(df / | awk 'NR==2 {print $5}' | sed 's/%//')

# Check if disk usage is above the threshold
if [ "$disk_usage" -gt "$threshold" ]; then
    # Email subject
    subject="Disk usage alert on $(hostname)"
    
    # Email body
    message="Disk usage on $(hostname) is above $threshold%. Current usage: $disk_usage%."

    # Send email to system admin
    echo "$message" | mail -s "$subject" amannarnaware8@gmail.com
fi

```
For Crontab

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/9aebde10-edbc-42fd-b7bd-26aa693f86a1)

---

### 3. write a shell script to take mysql database server backup. This script should run weekly on every sunday at 11:00 PM.

```
#!/bin/bash

# MySQL database information
db_user="root"
db_password="amanNBEAST8"
db_name="test"

# Backup directory
backup_dir="/home/aman/Desktop/Aman/Assignment2/backups"

# Date stamp for backup file
backup_date=$(date +%Y%m%d)

# MySQL dump command
mysqldump_cmd="mysqldump -u $db_user -p$db_password $db_name > $backup_dir/$db_name-$backup_date.sql"

# Execute MySQL dump command
eval "$mysqldump_cmd"

```
For crontab

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/81f9c245-9381-4b6b-a8cb-a7419b0a41c2)

**Output**

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/3e9cbcef-9e6e-4295-bc94-25e5b618a3f5)

---
