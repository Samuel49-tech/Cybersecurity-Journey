# Linux Notes
# Linux Notes

## Introduction

Linux is an open-source operating system widely used in servers, cybersecurity, cloud environments, and enterprise infrastructure. Many cybersecurity tools and platforms are built to run on Linux because of its flexibility, security, and command-line capabilities.

Learning Linux is important for SOC analysts, penetration testers, and system administrators because it allows better understanding of file systems, permissions, logs, networking, and system processes.

---

# Basic Linux Commands

## Checking Current Directory

```bash
pwd
```

Displays the current working directory.

Example:

```bash
/home/kali
```

---

## Listing Files and Directories

```bash
ls
```

Lists files in the current directory.

Useful options:

```bash
ls -la
```

* `-l` shows detailed information
* `-a` shows hidden files

---

## Changing Directories

```bash
cd directory_name
```

Example:

```bash
cd Downloads
```

Move back one directory:

```bash
cd ..
```

---

## Creating Files and Folders

Create a folder:

```bash
mkdir testfolder
```

Create a file:

```bash
touch notes.txt
```

---

## Viewing File Contents

Display file contents:

```bash
cat filename.txt
```

View large files page by page:

```bash
less filename.txt
```

---

# File Permissions

Linux permissions control who can read, write, or execute files.

Check permissions:

```bash
ls -l
```

Example:

```bash
-rwxr-xr--
```

Permission breakdown:

* `r` = read
* `w` = write
* `x` = execute

Modify permissions:

```bash
chmod 755 script.sh
```

---

# User Management

Check current user:

```bash
whoami
```

Switch user:

```bash
su username
```

Run commands as administrator:

```bash
sudo command
```

Example:

```bash
sudo apt update
```

---

# Package Management

Update package lists:

```bash
sudo apt update
```

Upgrade installed packages:

```bash
sudo apt upgrade
```

Install software:

```bash
sudo apt install nmap
```

---

# Networking Commands

Check IP address:

```bash
ip a
```

Test connectivity:

```bash
ping google.com
```

View active network connections:

```bash
netstat -tulnp
```

---

# Log Files

Linux stores logs mainly in:

```bash
/var/log/
```

Common logs:

* Authentication logs
* System logs
* Kernel logs

Example:

```bash
cat /var/log/auth.log
```

Logs are important during incident investigations and threat analysis.

---

# Processes

View running processes:

```bash
ps aux
```

Real-time process monitoring:

```bash
top
```

Terminate a process:

```bash
kill PID
```

---

# Key Takeaways

* Linux is heavily used in cybersecurity environments
* Command-line skills are essential for security analysts
* Understanding permissions, logs, networking, and processes helps during investigations
* Consistent Linux practice improves troubleshooting and system analysis skills
