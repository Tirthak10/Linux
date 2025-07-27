# 🐧 Linux Terminal Command Notes (Beginner-Friendly)

> A beginner-friendly reference sheet for essential Linux terminal commands.  
> Includes command descriptions, examples, use cases, and tips.

---

## 📍 1. `pwd` — Print Working Directory

**Description:**  
Displays the full path of your current location in the filesystem.

**Example:**
```bash
$ pwd
/home/tirthak/Desktop
```

**Use Case:**  
To check which directory you are currently working in.

---

## 📂 2. `ls` — List Directory Contents

**Description:**  
Lists files and directories inside the current working directory.

**Example:**
```bash
$ ls
Documents  Downloads  image.png  notes.txt
```

**Use Case:**  
To view what files and folders exist in the current location.

**Tip:**  
- `ls -l` → Long listing format with permissions  
- `ls -a` → Includes hidden files  
- `ls -lh` → Human-readable sizes

---

## 📁 3. `cd foldername` — Change Directory

**Description:**  
Moves you into a specified directory. Remember: **Linux is case-sensitive**.

**Example:**
```bash
$ cd Downloads
```

**Use Case:**  
Navigate deeper into folders to access or modify files.

**Note:**  
If the folder name is `Downloads`, `cd downloads` will not work.

---

## 🔙 4. `cd ..` — Move One Directory Up

**Description:**  
Moves you up one level to the parent directory.

**Example:**
```bash
$ cd ..
```

**Use Case:**  
Helpful when you want to go back one step in the folder hierarchy.

---

## ⌨️ 5. `TAB` Key — Autocomplete Shortcut

**Description:**  
Use the `TAB` key to auto-complete commands, folders, or file names.

**Example:**
```bash
$ cd Doc[TAB]
# Autocompletes to:
$ cd Documents
```

**Use Case:**  
Saves time and reduces typos.

**Also Works For:**  
- Commands (e.g., `gno[TAB]` → `gnome-text-editor`)

---

## 📦 6. `mkdir foldername` — Make Directory

**Description:**  
Creates a new directory (folder) in the current location.

**Example:**
```bash
$ mkdir Projects
```

**Use Case:**  
Organize your work by creating separate folders for different tasks.

---

## 📄 7. `touch filename` — Create Empty File

**Description:**  
Creates a new empty file. If the file exists, it updates its timestamp.

**Example:**
```bash
$ touch todo.txt
```

**Use Case:**  
Quickly create placeholder files to edit later.

---

## 📝 8. `gnome-text-editor filename` — Open GUI Text Editor

**Description:**  
Opens the specified file in GNOME's graphical text editor.

**Example:**
```bash
$ gnome-text-editor notes.txt
```

**Use Case:**  
To write or edit a file using a graphical interface.

**Shortcuts in Editor:**  
- Save: `Ctrl + S`  
- Exit: `Ctrl + Q`

**Tip:**  
Install with:
```bash
$ sudo apt install gnome-text-editor
```

---

## 🧹 9. `clear` — Clear Terminal Screen

**Description:**  
Clears all output from the terminal window.

**Example:**
```bash
$ clear
```

**Use Case:**  
To declutter the terminal for better readability.

**Shortcut:**  
- `Ctrl + L` does the same thing.

---

## 👁️ 10. `cat filename` — Display File Contents

**Description:**  
Prints the contents of a file directly in the terminal.

**Example:**
```bash
$ cat notes.txt
```

**Use Case:**  
To quickly read a file without opening it in an editor.

**Extra Tip:**  
You can merge files:
```bash
$ cat file1.txt file2.txt > combined.txt
```

---

## 🆘 11. `cat --help` — Help for `cat`

**Description:**  
Displays usage options and help for the `cat` command.

**Example:**
```bash
$ cat --help
```

**Use Case:**  
To understand all available flags for the command.

---

## 📘 12. `man command` — Manual Pages

**Description:**  
Displays the manual page for any command with detailed info.

**Example:**
```bash
$ man cat
```

**Use Case:**  
To deeply understand a command and its advanced usage.

**Navigation Tips:**  
- Scroll: Arrow Keys / Spacebar  
- Exit: Press `Q`

---

## 🧠 Bonus Tips & Shortcuts

| 🔑 Shortcut / Command | 🧰 Function                              |
|------------------------|------------------------------------------|
| `history`              | View command history                     |
| `!!`                   | Run the last command again               |
| `Ctrl + C`             | Cancel a running command                 |
| `Ctrl + D`             | Logout or close the terminal session     |
| `Ctrl + L`             | Clear the screen                         |
| `Ctrl + Shift + T`     | Open new terminal tab (GUI terminals)    |


---

> ✨ “Learning Linux is like gaining superpowers — the terminal is your wand!”

---
1. **`pwd`** (Print Working Directory): Displays the current working directory.

2. **`ls`** (List Directory Contents): Lists files and directories.

3. **`cd <foldername>`** (Change Directory): Navigates into a specified folder (case-sensitive).

4. **`cd ..`**: Moves up one level in the directory hierarchy.

5. **Tab-button**: A handy shortcut for auto-completing folder names or commands when navigating the terminal.
    * *Example*: Typing `cd Doc` and pressing **Tab** will auto-complete based on the current directory's content.
    * *Note*: This also works for commands.

6. **`mkdir <name of the directory>`**: Creates a new directory.

7. **`touch <filename>`**: Creates a new file.

8. **`gnome-text-editor <file.txt>`**: Opens the specified file in Gnome Text Editor for editing. (Save with Ctrl + S).

9. **`clear`**: Clears the terminal screen.

10. **`cat <name of the file>`**: Displays the content of a file.

11. **`cat --help`**: Provides a brief help message for the `cat` command.

12. **`man`**: Offers a more detailed manual page for commands. (Press **Q** to exit).

---

## History of Linux

Let’s go back to **1969**, when Ken Thompson and Dennis Ritchie of Bell Laboratories developed the **UNIX operating system**. It was later rewritten in C for greater portability and became widely used.

A decade later, Richard Stallman initiated the **GNU (GNU is Not UNIX) project**. While the GNU kernel, Hurd, unfortunately never came to completion, this effort led to the creation of the **GNU General Public License (GPL)**, a free software license.

The **kernel** is the most vital part of an operating system, enabling hardware to communicate with software. It controls almost everything on your system.

During this period, other UNIX-like systems like BSD and MINIX were developed, but they all lacked a unified kernel.

Then, in **1991**, Linus Torvalds began developing what we now know as the **Linux kernel**.

---

## 2. Choosing a Linux Distribution

The **Linux kernel** powers millions of devices daily. While "Linux" often refers to the kernel, many distributions use the Linux kernel and are commonly known as Linux operating systems.

A Linux system consists of three main parts:

- **Hardware**: Includes all physical components like memory, CPU, and disks.
- **Linux Kernel**: The core of the operating system, managing hardware interactions.
- **User Space**: Where users directly interact with the system.

The first step is installing Linux. This course will guide you in choosing a suitable distribution. We'll cover the most popular options.

---

## 3. Debian

**Overview**
Debian is an operating system entirely composed of **free and open-source software**. It has been in development for over 20 years and is widely recognized. You can choose from three branches: **Stable**, **Testing**, and **Unstable**.

Stable is generally recommended. Testing and Unstable are rolling releases, meaning incremental changes in these branches will eventually transition to Stable. For example, upgrading from Windows XP to Windows 10 requires a full installation, but on a Testing release, updates are automatically received until it becomes the next stable OS without needing a full reinstallation.

**Package Management**
Debian uses its own **Debian package management tools**. Different Linux distributions utilize various package managers, a topic we'll explore further in a later course.

**Configurability**
While Debian might not receive the absolute latest updates, it is **extremely stable**. If you desire a robust "core" operating system, Debian is an excellent choice.

**Uses**
Debian is a versatile operating system suitable for **any platform**.

---

## 4. Red Hat Enterprise Linux

**Overview**
**Red Hat Enterprise Linux (RHEL)**, developed by Red Hat, has strict rules restricting free re-distribution, though its source code is freely available.

**Package Management**
RHEL employs a different package manager than Debian: the **RPM package manager**, which we will also cover.

**Configurability**
RHEL-based operating systems differ slightly from Debian-based ones, primarily in package management. If you plan to work with RHEL, choosing it as your primary OS is advisable.

**Uses**
As its name suggests, RHEL is primarily used in **enterprise environments**, making it a strong choice for a reliable server OS.

---

## 5. Ubuntu

**Overview**
**Ubuntu** is one of the most popular Linux distributions for personal machines. It ships with its own desktop environment manager, Unity, by default.

**Package Management**
As a **Debian-based operating system** developed by Canonical, Ubuntu uses a core Debian package management system.

**Configurability**
Ubuntu is an excellent starting point for Linux beginners. Its ease of use and great user interface have contributed to its widespread adoption. It's widely used and supported, offering a usability experience similar to macOS and Windows.

**Uses**
Great for **any platform**: desktop, laptop, and server.

---

## 6. Fedora

**Overview**
Backed by Red Hat, the **Fedora Project** is a community-driven initiative featuring open-source and free software. Red Hat Enterprise Linux branches off Fedora, so consider Fedora an "upstream" RHEL operating system. RHEL eventually incorporates updates from Fedora after extensive testing and quality assurance. Think of Fedora as an Ubuntu equivalent, but with a Red Hat backend instead of Debian.

**Package Management**
Uses the **Red Hat package manager**.

**Configurability**
If you prefer a Red Hat-based operating system, Fedora offers a **user-friendly version**.

**Uses**
Fedora is ideal if you want a Red Hat-based operating system without the associated price tag. Recommended for **desktop and laptop use**.

---

## 7. Linux Mint

**Overview**
**Linux Mint** is based on Ubuntu and utilizes Ubuntu’s software repositories, making the same packages available on both distributions. If you're looking for a lighter distribution than Ubuntu, Linux Mint might be of interest.

**Package Management**
Since Linux Mint is Ubuntu-based, it uses the **Debian package manager**.

**Configurability**
Linux Mint offers a **great user interface**, is excellent for beginners, and is less bloated than Ubuntu. This course will use Linux Mint, but any other distribution can be used.

**Uses**
Great for **desktop and laptop use**.

---

## 8. Gentoo

**Overview**
**Gentoo** offers unparalleled flexibility with the operating system, but at a price. It's designed for advanced users who are comfortable with in-depth system configuration.

**Package Management**
Gentoo uses its own package management system, **Portage**. Portage is highly modular and easy to maintain, which significantly contributes to the operating system's overall flexibility.

**Configurability**
If you're new to Linux and want to take a more challenging path, consider Gentoo or Arch Linux as your distribution.

**Uses**
Great for **desktop and laptop use**.

---

## 9. Arch Linux

**Overview**
**Arch Linux** is a lightweight and flexible distribution driven entirely by its community. Similar to Debian, Arch uses a **rolling release model**, where incremental updates eventually become the stable release. You'll need to delve deep into the system to understand its functions, but in return, you gain complete and total control.

**Package Management**
It uses its own package manager, **Pacman**, for installing, updating, and managing packages.

**Configurability**
If you want a lightweight operating system and genuinely want to understand Linux, use Arch! There's a learning curve, but for hardcore Linux users, it's an excellent choice.

**Uses**
Great for **desktop and laptop use**. It's also perfect for small devices like a Raspberry Pi when you need a lightweight OS.

---

## 10. openSUSE

**Overview**
**openSUSE Linux** is developed by the openSUSE Project, a community that promotes Linux usage worldwide through open, transparent, and friendly collaboration within the Free and Open Source Software community. openSUSE is the second oldest still-running Linux distribution and shares its base system with SUSE's acclaimed SUSE Linux Enterprise products.

**Package Management**
Uses the **RPM package manager**.

**Configurability**
openSUSE is a great choice for new Linux users. It provides an easy-to-use graphical installer/administration application ([YaST](http://yast.github.io/)) and a tidy base system that's easy to tinker with. openSUSE includes everything needed for secure internet use and to fuel your creativity with photos, videos, music, or code.

**Uses**
openSUSE Leap is fully capable of being used on **desktop PCs and laptops**.

---

# Navigating the File System

Here are explanations and examples of essential commands for file system navigation:

* **`pwd`** (Print Working Directory):
    * *Explanation*: Displays the current working directory's absolute path.
    * *Example*: Running `pwd` might show `/home/user/documents`.

* **`cd`** (Change Directory):
    * *Explanation*: Allows you to change your current working directory.
    * *Example*: `cd /home/user/documents` changes the directory.

* **`cd ..`** (Change to Parent Directory):
    * *Explanation*: Moves up one level in the directory hierarchy.
    * *Example*: From `/home/user/documents`, `cd ..` moves to `/home/user`.

* **`ls`** (List Directory Contents):
    * *Explanation*: Lists files and directories in the current directory.
    * *Example*: `ls` displays the contents.

* **`ls -la`** (List Detailed Directory Contents):
    * *Explanation*: Lists detailed information about files and directories, including hidden ones.
    * *Example*: `ls -la` shows a comprehensive list.

* **`mkdir`** (Make Directory):
    * *Explanation*: Creates a new directory.
    * *Example*: `mkdir new_folder` creates a directory named "new_folder".

* **`rmdir`** (Remove Directory):
    * *Explanation*: Removes an *empty* directory.
    * *Example*: `rmdir empty_folder` removes "empty_folder" if it's empty.

* **`man`** (Manual):
    * *Explanation*: Displays the manual pages for a specified command, offering detailed information.
    * *Example*: `man ls` shows the manual for the `ls` command.

* **`echo`**:
    * *Explanation*: Displays text or variables as output.
    * *Example*: `echo "Hello, world!"` outputs "Hello, world!".

* **`>`** (Output Redirection):
    * *Explanation*: Redirects a command's output to a file, overwriting it if it exists.
    * *Example*: `echo "Hello" > greeting.txt` writes "Hello" to `greeting.txt`.

* **`>>`** (Append Output):
    * *Explanation*: Redirects a command's output and appends it to a file.
    * *Example*: `echo "World!" >> greeting.txt` adds "World!" to the end of `greeting.txt`.

* **`rm`** (Remove):
    * *Explanation*: Deletes files or directories.
    * *Example*: `rm file.txt` deletes "file.txt".

* **`mv`** (Move):
    * *Explanation*: Moves or renames files and directories.
    * *Example*: `mv file.txt new_directory/file_renamed.txt` moves and renames the file.

* **`cp`** (Copy):
    * *Explanation*: Copies files and directories.
    * *Example*: `cp file.txt backup/file_copy.txt` creates a copy in the "backup" directory.

* **`locate`**:
    * *Explanation*: Searches for files and directories using a prebuilt database.
    * *Example*: `locate myfile.txt` searches for "myfile.txt".

* **`updatedb`**:
    * *Explanation*: Updates the `locate` command's database to reflect recent file system changes.
    * *Example*: `updatedb` updates the database for current search results.

* **`passwd`**:
    * *Explanation*: Allows a user to change their password.
    * *Example*: `passwd` prompts for current and new passwords.

**Caution**: Exercise extreme care with commands like `rm`, as they can permanently delete files. Always double-check before executing them.

---

# User and Privileges

In the **`ls -la`** output, "rwx" indicates file or directory permissions for three entities: **owner**, **group**, and **other users**. Each entity has three permission categories: **read (r)**, **write (w)**, and **execute (x)**.

* **Read (r)**: Allows viewing file contents or directory names.
* **Write (w)**: Enables modifying files or adding/deleting/renaming files within a directory.
* **Execute (x)**: Grants permission to run a file or enter a directory. For directories, execute permission is crucial for accessing their contents.

The `ls -la` output displays permissions as nine characters. The first character denotes the file type (`-` for a regular file, `d` for a directory). The next three characters are for the owner, followed by three for the group, and then three for other users.

**Example `ls -la` output line**:
`-rwxr-x--- 1 user group 4096 May 10 12:34 myfile.txt`

Here's the breakdown:

* **`-rwxr-x---`**:
    * First character (`-`): Regular file.
    * Next three (`rwx`): Owner has read, write, and execute permissions.
    * Next three (`r-x`): Group has read and execute permissions.
    * Last three (`---`): Other users have no permissions.
* **`1`**: Number of hard links to the file.
* **`user`**: File owner.
* **`group`**: Group assigned to the file.
* **`4096`**: File size in bytes.
* **`May 10 12:34`**: Date and time of last modification.
* **`myfile.txt`**: File name.

A hyphen (`-`) indicates that a permission is not granted. The output may also include special permissions, ownership, and timestamps.

Here are explanations and examples of the commands related to users and privileges:

* **`chmod`** (Change Mode):
    * *Explanation*: Changes a file or directory's permissions.
    * *Example*: `chmod +x script.sh` adds execute permission to "script.sh".

* **`adduser`**:
    * *Explanation*: Creates a new user account.
    * *Example*: `adduser john` creates "john" and prompts for details.

* **`su`** (Switch User):
    * *Explanation*: Allows switching to another user account.
    * *Example*: `su jane` switches to "jane" after password entry.

* **`/etc/sudoers`**:
    * *Explanation*: Displays the content of the `/etc/sudoers` file, which configures the `sudo` command.
    * *Example*: Running this command shows `sudo` access and permission directives.

* **`sudo -l`**:
    * *Explanation*: Lists commands a user is permitted to run with `sudo` privileges.
    * *Example*: `sudo -l` displays available commands and permissions for the current user with `sudo` access.

**Note**: Some of these commands require administrative privileges. Exercise caution when modifying system files or managing user accounts.

---

# Common Network Commands

Here are explanations and examples of common network commands:

* **`ip a`**:
    * *Explanation*: Displays network interfaces and their associated IP addresses.
    * *Example*: `ip a` shows IP addresses, MAC addresses, and other details for network interfaces.

* **`ifconfig`**:
    * *Explanation*: Displays the configuration and status of network interfaces.
    * *Example*: `ifconfig` shows IP addresses, MAC addresses, and other information for active network interfaces.

* **`iwconfig`**:
    * *Explanation*: Displays the configuration and status of wireless network interfaces.
    * *Example*: `iwconfig` shows wireless signal strength, frequency, and encryption for active wireless interfaces.

* **`ip n`**:
    * *Explanation*: Displays the Neighbor Table (ARP cache), containing IP-to-MAC address mappings for local network devices.
    * *Example*: `ip n` shows IP and MAC addresses of recently communicating devices.

* **`arp -a`**:
    * *Explanation*: Displays the ARP (Address Resolution Protocol) cache, which maps IP addresses to MAC addresses.
    * *Example*: `arp -a` shows IP and MAC addresses resolved recently by ARP.

* **`ip r`**:
    * *Explanation*: Displays the routing table, which contains information about network routes.
    * *Example*: `ip r` shows destination networks, gateway IP addresses, and network interfaces.

* **`route`**:
    * *Explanation*: Displays or manipulates the IP routing table.
    * *Example*: `route` displays the routing table, similar to `ip r`.

* **`ping`**:
    * *Explanation*: Sends ICMP echo requests to a specified IP address to check network connectivity and measure round-trip time.
    * *Example*: `ping 8.8.8.8` sends requests to Google's DNS server and displays statistics.

These commands are frequently used for network troubleshooting, configuration, and gathering network-related information in Linux systems.

---

# Viewing, Creating, and Editing Files

Here are explanations and examples of commands for file manipulation:

* **`echo "hello" > hey.txt`**:
    * *Explanation*: Creates or overwrites `hey.txt` with the content "hello".
    * *Example*: Writes "hello" into `hey.txt`.

* **`echo "hello again" >> hey.txt`**:
    * *Explanation*: Appends "hello again" to `hey.txt`, or creates the file if it doesn't exist.
    * *Example*: Adds "hello again" to the end of `hey.txt`.

* **`touch newfile.txt`**:
    * *Explanation*: Creates an empty `newfile.txt` or updates an existing file's timestamp to the current time.
    * *Example*: Creates "newfile.txt" or updates its last modified time.

* **`nano newfile.txt`**:
    * *Explanation*: Opens the Nano text editor to create or edit `newfile.txt`.
    * *Example*: Launches Nano, allowing text entry or modification in "newfile.txt".

* **`mousepad newfile.txt`**:
    * *Explanation*: Opens the Mousepad text editor to create or edit `newfile.txt`.
    * *Example*: Launches Mousepad for editing "newfile.txt".

These commands are commonly used for basic file manipulation and editing within Linux. `echo` prints text or redirects it to files, `touch` creates or updates file timestamps, and `nano` and `mousepad` are terminal-based text editors.

---

# Installing and Updating Tools

Here are explanations and examples of commands for managing software in Linux:

* **`sudo apt update && sudo apt upgrade`**:
    * *Explanation*: Updates package lists and upgrades installed packages on Debian-based Linux systems using the APT package manager.
    * *Example*: Fetches information about available updates and then upgrades existing software to their latest versions.

* **`sudo apt install cron-daemon-common`**:
    * *Explanation*: Installs the "cron-daemon-common" package using APT. This package provides common files and utilities for the `cron-daemon`, a time-based job scheduler.
    * *Example*: Downloads and installs "cron-daemon-common" on the system.

* **`sudo git clone https://github.com/Dewalt-arch/pimpmykali.git`**:
    * *Explanation*: Clones a Git repository from the specified URL using the Git version control system.
    * *Example*: Creates a local copy of the repository's files and version history from the given URL.

These commands are frequently used in Linux for maintaining system software, installing new applications, and working with version-controlled code repositories. The **`sudo`** command grants superuser privileges, **`apt`** manages packages on Debian-based distributions, and **`git`** is used for version control.

---

# Scripting and Bash

Here's an example of a simple bash script:

```bash
#!/bin/bash

if [ "$1" == "" ]
then
    echo "You forgot an IP address!"
    echo "Syntax: ./ipsweep.sh 192.168.1"
else
    for ip in `seq 1 254`; do
        ping -c 1 $1.$ip | grep "64 bytes" | cut -d " " -f 4 | tr -d ":" &
    done
fi

```
---
## 🙋‍♂️ Author

**Tirthak Likhar**  
🔗 [LinkedIn](https://www.linkedin.com/in/tirthak-likhar-8808a8255/)  
💻 [GitHub](https://github.com/)

---
