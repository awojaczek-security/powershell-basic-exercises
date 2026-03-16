

# 📄 Hacking with Powershell - Answers to questions about Enumeration

---

## 🧠 SUMMARY

This article describes the basic commands used in the Powershell shell and solves exercises from the TryHackMe - Hacking with Powershell course.

In conclusion, **PowerShell** is a very important tool in modern IT environments. Its flexibility, scripting capabilities, and integration with system components make it a valuable resource for system administrators, DevOps engineers, and cybersecurity professionals. The completed tasks helped build practical skills and a deeper understanding of how PowerShell can be used in real-world situations.

## 🔎 PowerShell - What is it? - the most important informations

**PowerShell** is a command-line shell and scripting language developed by Microsoft, used for automating tasks, system administration, and environment configuration, primarily on Microsoft Windows.

**Key Information**

PowerShell is used for:

- administering Microsoft Windows systems

- automating tasks (e.g., installations, configurations)

- managing files and folders

- managing servers and networks

- writing administrative scripts


**PowerShell** runs in a terminal, similar to:

- Command Prompt (CMD)

- Linux Bash

But it is **more advanced**.

## 💡 The Most Important PowerShell Commands

1. **Get-Help**

- Displays documentation and usage information for PowerShell commands.

Example:

*Get-Help Get-Process*

This command shows instructions and details about how the Get-Process command works.

2. **Get-Command**

- Lists available commands in PowerShell.

Example:

*Get-Command*

It displays all commands that can be executed in the current PowerShell environment.

3. **Get-Process**

- Shows all processes that are currently running on the system.

Example:

*Get-Process*

This command provides information about active programs and background processes.

4. **Get-Service**

- Displays services installed on the system and their current status.

Example:

*Get-Service*

It allows administrators to check whether services are running or stopped.

5. **Get-ChildItem**

- Lists files and directories in a specified location.

Example:

Get-ChildItem

This command shows the contents of the current directory, similar to dir or ls.

6. **Set-Location**

- Changes the current working directory.

Example:

*Set-Location C:\Users*

It moves the user to the specified folder.

7. **Copy-Item**

- Copies files or directories from one location to another.

Example:

*Copy-Item file.txt C:\Backup*

This command creates a copy of file.txt in the Backup folder.

8. **Remove-Item**

- Deletes files or directories.

Example:

*Remove-Item file.txt*

It permanently removes the specified file.

9. **New-Item**

- Creates new files or folders.

Example:

*New-Item test.txt*

This command creates a new file called test.txt.

10. **Stop-Process**

- Terminates a running process.

Example:

*Stop-Process -Name notepad*

This command stops the Notepad application if it is currently running.


## 🔥 **Answers the guestions**:

The first step when you have gained initial access to any machine would be to enumerate. We'll be enumerating the following:

- users
- basic networking information
- file permissions
- registry permissions
- scheduled and running tasks
- insecure files

1. How many users are there on the machine?

</p>
<p align="center">
  <img src="../01_Ans_1/Path_to_file.png" width="600">
  <br>
  <em>Figure 1: Answer 1 - Path_to_file</em>
</p>

2. Which local user does this SID(S-1-5-21-1394777289-3961777894-1791813945-501) belong to?
3. How many users have their password required values set to False?
4. How many local groups exist?
5. What command did you use to get the IP address info?
6. How many ports are listed as listening?
7. What is the remote address of the local port listening on port 445?
8. How many patches have been applied?
9. When was the patch with ID KB4023834 installed?
10. Find the contents of a backup file.
11. Search for all files containing API_KEY
12. What command do you do to list all the running processes?
13. What is the path of the scheduled task called new-sched-task?
14. Who is the owner of the C:\

**The Summary of the investigation**:

This report presents answers and solutions related to tasks from the Hacking with PowerShell course. The main goal of the work was to understand the basic concepts of using PowerShell and to practice the most important commands used in system administration and cybersecurity.

During the exercises, various PowerShell commands were used to explore system processes, services, files, and directories. The tasks also demonstrated how PowerShell can be applied in practical scenarios related to system management and security analysis.


Working with these exercises helped develop a better understanding of how command-line tools operate and how automation can simplify complex administrative tasks. 

## 📂 Project Structure

```bash
PowerShell_Excercise_1
│
├── 00_README
│   └── README.md
│


```



