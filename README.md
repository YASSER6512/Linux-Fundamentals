# Linux-Fundamentals
### Linux File System & Key Commands for Ethical Hacking

Welcome to my Linux Fundamentals repository! This project provides an overview of the Linux file system architecture and the essential commands used in system administration and ethical hacking. 

### 1. Linux File System Overview

The Linux file system structure is entirely different from Windows. Instead of drive letters (like C: or D:), Linux uses a unified, hierarchical directory structure. 

* *The Root Directory (/)*: This is the top-level directory of the entire system. Every other directory, file, or storage drive stems from this single root (/).
* *Tree Hierarchy*: The file system expands downward like an inverted tree starting from the root directory.
* *Everything is a File: One of the core philosophies of Linux is that *everything is a file. Whether it is a text document, a folder, a hard drive, or a network interface, the operating system treats and manages it as a file.

### 2. Important Directories for Ethical Hacking

Understanding specific Linux directories is vital for penetration testing, security auditing, and system analysis: 

* */etc* 

  * *Purpose*: Contains system configuration files.
  * *Hacking Relevance*: Critical files like /etc/passwd (user account list) and /etc/shadow (encrypted user passwords) are primary targets during password cracking or privilege escalation practice.
* */var/log* 

  * *Purpose*: Stores system, authentication, and application log files.
  * *Hacking Relevance*: Security analysts review these logs to track malicious activities, while penetration testers check them to understand how their actions are being recorded.
* */tmp* 

  * *Purpose*: A temporary folder used by the system and applications to store temporary data.
  * *Hacking Relevance*: This folder usually grants global write and execute permissions (rwxrwxrwt) to any user. Attackers often use it to download and run exploit scripts or payloads.
* */bin & /sbin* 

  * *Purpose*: Contains essential binary executables (system commands). /bin contains general user commands, while /sbin holds system administrative commands.
  * *Hacking Relevance*: These folders contain fundamental tools used for system interaction, network configuration (ifconfig, ip), and post-exploitation tasks.

### 3. Essential Linux Commands Reference

Command 

Description 

Example Usage 

*pwd*
Prints the path of the current working directory.pwd
*ls*
Lists files and directories within a folder.ls -la /etc
*cd*
Changes the current working directory.cd /var/log
*cat*
Concatenates and displays file contents in the terminal.cat /etc/passwd
*chmod*
Modifies file or directory permissions (read, write, execute).chmod +x script.sh
*sudo*
Executes a command with administrative (root) privileges.sudo apt update

### 4. Assignment Completion Status

* *Linux Tasks*: Successfully explored the root directory (/), listed system files using ls -la, and analyzed user details via cat /etc/passwd.
* *GitHub Repository*: Created this repository and successfully documented all the learnings in this README file.
* *LinkedIn Post*: Shared the learning journey and key Linux insights with the professional community.

Disclaimer: This repository is created strictly for educational purposes and academic assessment.
