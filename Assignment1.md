# Assignment - 1
## Study Linux Commands

>Name: Aman Narnaware
>
>Roll: 322005
>
>Batch: B1
>
>PRN: 22110404

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

### 14. ifconfig - configure a network interface

```
ifconfig [-v] [-a] [-s] [interface]
ifconfig [-v] interface [aftype] options | address ...
```

**Description**

Ifconfig  is used to configure the kernel-resident network interfaces.  It is used at boot time to set up interfaces as necessary.  After that, it is usually only needed when debugging or when system  tun‐ ing is needed.

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/0a3dc264-2f56-4493-a6e1-a2f66035f1fa)

---

### 15. ip - show / manipulate routing, network devices, interfaces and tunnels

```
ip [ OPTIONS ] OBJECT { COMMAND | help }
ip [ -force ] -batch filename
```

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/10b6f76a-d810-427b-96dd-162b1a91dd52)

---

### 16. sudo, sudoedit — execute a command as another user

```
sudo -h | -K | -k | -V
       sudo -v [-ABkNnS] [-g group] [-h host] [-p prompt] [-u user]
       sudo -l [-ABkNnS] [-g group] [-h host] [-p prompt] [-U user] [-u user] [command [arg ...]]
       sudo  [-ABbEHnPS]  [-C  num]  [-D directory] [-g group] [-h host] [-p prompt] [-R directory] [-r role]
           [-t type] [-T timeout] [-u user] [VAR=value] [-i | -s] [command [arg ...]]
       sudoedit [-ABkNnS] [-C num] [-D directory] [-g group] [-h host] [-p prompt] [-R directory]  [-r  role]
            [-t type] [-T timeout] [-u user] file ...
```

**Description**

sudo  allows  a  permitted user to execute a command as the superuser or another user, as specified by the security policy.  The invoking user's real (not effective) user-ID is used to determine  the  user name with which to query the security policy.

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/54433b3c-10f0-4a90-8bf4-4587eaf99e53)

---

### 17. apt - command-line interface

```
apt [-h] [-o=config_string] [-c=config_file] [-t=target_release] [-a=architecture] {list | search |
           show | update | install pkg [{=pkg_version_number | /target_release}]...  | remove pkg...  |
           upgrade | full-upgrade | edit-sources | {-v | --version} | {-h | --help}}
```

**Description**

apt provides a high-level commandline interface for the package management system. It is intended as an end user interface and enables some options better suited for interactive usage by default compared to more specialized APT tools like apt-get(8) and apt-cache(8).

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/06dd9acd-ff50-4852-9d9f-2b2ac23dbab5)

---

### 18. mv - move (rename) files

```
mv [OPTION]... [-T] SOURCE DEST
mv [OPTION]... SOURCE... DIRECTORY
mv [OPTION]... -t DIRECTORY SOURCE...
```

**Description**

Rename SOURCE to DEST, or move SOURCE(s) to DIRECTORY.

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/af0ade0b-00ae-4060-a6e8-3203d26123ad)

---

### 19. cp - copy files and directories

```
cp [OPTION]... [-T] SOURCE DEST
cp [OPTION]... SOURCE... DIRECTORY
cp [OPTION]... -t DIRECTORY SOURCE...
```

**Description**

Copy SOURCE to DEST, or multiple SOURCE(s) to DIRECTORY.

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/283697a7-e633-46fc-88e9-f63fbc0983f6)

---

### 20. ln - make links between files

```
ln [OPTION]... [-T] TARGET LINK_NAME
ln [OPTION]... TARGET
ln [OPTION]... TARGET... DIRECTORY
ln [OPTION]... -t DIRECTORY TARGET...
```

**Description**

In  the  1st form, create a link to TARGET with the name LINK_NAME.  In the 2nd form, create a link to TARGET in the current directory.  In the 3rd and 4th forms, create links to each TARGET in  DIRECTORY. Create  hard  links by default, symbolic links with --symbolic.  By default, each destination (name of new link) should not already exist.  When creating hard links, each TARGET must exist.  Symbolic links can hold arbitrary text; if later resolved, a relative link is interpreted in relation to  its  parent directory.

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/c6dec566-bb7d-478a-a715-6ae386b8b480)

---

### 21. rm - remove files or directories

```
rm [OPTION]... [FILE]...
```

**Description**

rm removes each specified file.  By default, it does not remove directories.

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/36c4424b-4d74-4d04-bab8-a7811a83b7fe)

---

### 22. rmdir - remove empty directories

```
rmdir [OPTION]... DIRECTORY...
```

**Description**

Remove the DIRECTORY(ies), if they are empty.

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/3260d048-330b-43df-917a-7ca227f5263b)

---

### 23. mkdir - make directories

```
mkdir [OPTION]... DIRECTORY...
```

**Description**

Create the DIRECTORY(ies), if they do not already exist.

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/80992be9-b7c2-4f25-bd19-e747870a9503)

---

### 24. man - an interface to the system reference manuals

```
man [man options] [[section] page ...] ...
man -k [apropos options] regexp ...
man -K [man options] [section] term ...
man -f [whatis options] page ...
man -l [man options] file ...
man -w|-W [man options] page ...
```

**Description**

man  is the system's manual pager.  Each page argument given to man is normally the name of a program, utility or function.  The manual page associated with each of these arguments is then found  and  dis‐ played.   A section, if provided, will direct man to look only in that section of the manual.  The de‐ fault action is to search in all of the available sections following  a  pre-defined  order  (see  DE‐ FAULTS), and to show only the first page found, even if page exists in several sections.

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/4d945051-6ede-43e0-a4c4-5ecec08cfedc)
> man ls

---

### 25. head - output the first part of files

```
head [OPTION]... [FILE]...
```

**Description**

Print  the first 10 lines of each FILE to standard output.  With more than one FILE, precede each with a header giving the file name.

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/e7b26db8-6564-4fe4-b1f4-c7444648885b)

---

### 26. tail - output the last part of files

```
tail [OPTION]... [FILE]...
```

**Description**

Print the last 10 lines of each FILE to standard output.  With more than one FILE, precede each with a header giving the file name.

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/fea61367-e251-4887-91ef-cc64092d239a)

---

### 27. chmod - change file mode bits

```
chmod [OPTION]... MODE[,MODE]... FILE...
chmod [OPTION]... OCTAL-MODE FILE...
chmod [OPTION]... --reference=RFILE FILE...
```

**Description**

chmod changes the file mode bits of each given file according to mode, which can be either a symbolic representation of changes to make, or an  octal number representing the bit pattern for the new mode bits.

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/92005332-f311-4cee-9d23-1a9ff9ab3806)

---

### 28. pwd - print name of current/working directory

```
pwd [OPTION]...
```

**Description**

Print the full filename of the current working directory.

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/68c37281-8093-41ff-b9e2-1de5f8f2181c)

---

### 29. Wget - The non-interactive network downloader.

```
wget [option]... [URL]...
```

**Description**

GNU Wget is a free utility for non-interactive download of files from the Web.  It supports HTTP, HTTPS, and FTP protocols, as well as retrieval through HTTP proxies.

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/e2afa823-cd36-486c-a9bf-eafb7c53fc7d)

---

### 30. gzip, gunzip, zcat - compress or expand files

```
gzip [ -acdfhklLnNrtvV19 ] [-S suffix] [ name ...  ]
gunzip [ -acfhklLnNrtvV ] [-S suffix] [ name ...  ]
zcat [ -fhLV ] [ name ...  ]
```

**Description**

The  gzip command reduces the size of the named files using Lempel-Ziv coding (LZ77).  Whenever possi‐ ble, each file is replaced by one with the extension .gz, while keeping the same ownership modes,  ac‐ cess  and  modification  times.   (The  default extension is z for MSDOS, OS/2 FAT, Windows NT FAT and Atari.)  If no files are specified, or if a file name is "-", the standard input is compressed to  the standard  output.   The  gzip  command will only attempt to compress regular files.  In particular, it will ignore symbolic links.

![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/db4db0fc-0e78-4143-84ae-adec1c980538)

---
