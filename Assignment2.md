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

2. Different types of shells

In the Linux and Unix environments, there are several types of shells available, each with its own features and capabilities. Some of the most common types of shells include:

a. **Bourne Shell (sh):** Developed by Stephen Bourne at AT&T's Bell Labs, the Bourne Shell is one of the oldest Unix shells. It provides basic functionality for executing commands, scripting, and control flow structures like loops and conditionals.

b. **Bourne-Again Shell (bash):** Bash is the default shell for most Linux distributions. It is backward-compatible with the Bourne Shell but includes additional features such as command-line editing, history, and job control. Bash is highly customizable and widely used by both casual users and system administrators.

c. **C Shell (csh):** Developed by Bill Joy at the University of California, Berkeley, the C Shell features a C-like syntax and interactive command-line editing. It introduced several innovative features at the time, such as history substitution and aliases.

d. **Korn Shell (ksh):** Developed by David Korn at Bell Labs, the Korn Shell combines features from the Bourne Shell and the C Shell while introducing its own enhancements. It offers advanced scripting capabilities, command-line editing, and programmable completion.

e. **Z Shell (zsh):** Zsh is an extended Bourne Shell with additional features for interactive use and scripting. It includes powerful tab completion, spelling correction, and advanced customization options. Zsh is highly configurable and often preferred by power users.

