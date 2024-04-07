# Assignment - 1
## Study Linux Commands

### 1. cat - concatenate files and print on the standard output

```
cat [OPTION]... [FILE]...
```

**Description**

Concatenate FILE(s) to standard output.
With no FILE, or when FILE is -, read standard input.

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/636024ec-763e-4fe9-80ab-a8dd2c7e3fdf)

---

### 2. touch - change file timestamps

```
touch [OPTION]... FILE...
```

**Description**

Update the access and modification times of each FILE to the current time.
A FILE argument that does not exist is created empty, unless -c or -h is supplied.

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/1be11248-7383-40d6-bbe5-7c5787bc4371)

---

### 3. top - display linux processes

```
top [options]
```

**Description**

The  top program provides a dynamic real-time view of a running system.  It can display system summary information as well as a list of processes or threads currently being managed  by  the  Linux  kernel.

The  types  of system summary information shown and the types, order and size of information displayed for processes are all user configurable and that configuration can be made persistent across restarts.

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/f5a1e19d-2db0-44bd-874a-6b3201bf5ffa)

---

### 4. ls - list directory contents

```
ls [OPTION]... [FILE]...
```

**Description**

List  information  about the FILEs (the current directory by default).  Sort entries alphabetically if none of -cftuvSUX nor --sort is specified.

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/33b1c621-bfb8-4513-86b6-5dd2789f1a3b)

---

### 5. clear - clear the terminal screen

```
clear [-x] [-T type]
```

**Description**

clear  clears  your terminal's screen and its scrollback buffer, if any.  clear retrieves the terminal type from the environment variable TERM, then consults the terminfo terminal capability database entry for that type to determine how to perform these actions.


---

### 6. systemctl - Control the systemd system and service manager

```
systemctl [OPTIONS...] COMMAND [UNIT...]
```

**Description**

systemctl may be used to introspect and control the state of the "systemd" system and service manager.

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/5ea50517-5fa4-472a-9b83-8d6b96c4e16c)

---

### 7. passwd - change user password

```
passwd [options] [LOGIN]
```

**Description**

The passwd command changes passwords for user accounts. A normal user may only change the password for their own account, while the superuser may change the password for any account.  passwd also changes the account or associated password validity period.

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/769a895f-f006-43bf-9dca-307dbe066bf1)

---

### 8. echo - display a line of text

```
echo [SHORT-OPTION]... [STRING]...

echo LONG-OPTION
```

**Description**

Echo the STRING(s) to standard output.

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/224a3ef1-ae9d-4863-9815-90deed0a7161)

---

### 9. base64 - base64 encode/decode data and print to standard output

```
base64 [OPTION]... [FILE]
```

**Description**

Base64 encode or decode FILE, or standard input, to standard output. With no FILE, or when FILE is -, read standard input.

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/3d1dd124-1d08-4ee7-a7f0-8ee812c7520d)

---

### 10. grep, egrep, fgrep, rgrep - print lines that match patterns

```
grep [OPTION...] PATTERNS [FILE...]

grep [OPTION...] -e PATTERNS ... [FILE...]

grep [OPTION...] -f PATTERN_FILE ... [FILE...]
```

**Description**

grep  searches  for  PATTERNS  in  each  FILE.   PATTERNS is one or more patterns separated by newline characters, and grep prints each line that matches a pattern.  Typically  PATTERNS  should  be  quoted when grep is used in a shell command.

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/fd3a0fa1-d1af-4010-a7a0-c72c9a1aab56)

---

### 11. who - show who is logged on

```
who [OPTION]... [ FILE | ARG1 ARG2 ]
```

**Description**

Print information about users who are currently logged in.

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/43a2f04e-01e9-4046-b982-5016bf2d20c3)

---

### 12. whoami - print effective user name

```
whoami [OPTION]...
```

**Description**

Print the user name associated with the current effective user ID.  Same as id -un.

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/91113c8f-7f75-44a5-8cfa-edc8473c1035)

---

### 13. ssh — OpenSSH remote login client

```
ssh    [-46AaCfGgKkMNnqsTtVvXxYy]    [-B    bind_interface]   [-b   bind_address]   [-c   cipher_spec]
           [-D  [bind_address:]port]  [-E  log_file]   [-e   escape_char]   [-F   configfile]   [-I   pkcs11]
           [-i  identity_file]  [-J  destination]  [-L  address]  [-l  login_name] [-m mac_spec] [-O ctl_cmd]
           [-o option] [-P tag] [-p port]  [-Q  query_option]  [-R  address]  [-S  ctl_path]  [-W  host:port]
           [-w local_tun[:remote_tun]] destination [command [argument ...]]
```

**Description**

ssh (SSH client) is a program for logging into a remote machine and for executing commands on a remote machine.   It  is intended to provide secure encrypted communications between two untrusted hosts over an insecure network.  X11 connections, arbitrary TCP ports and Unix-domain sockets can  also  be  for‐ warded over the secure channel.

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/8c89ace1-2cd8-4523-aec1-5d52511ce27e)

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/5ae6c278-0477-4d04-a0aa-23881ec65d67)

---
