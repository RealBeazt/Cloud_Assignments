# Assignment - 2
## Shell Scripting

>Name: Aman Narnaware
>
>Roll: 322005
>
>Batch: B1
>
>PRN: 22110404

1. What is Shell (Linux kernel architecture diagram)
   
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

