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

## 🙋‍♂️ Author

**Tirthak Likhar**  
🔗 [LinkedIn](https://www.linkedin.com/in/tirthak-likhar-8808a8255/)  
💻 [GitHub](https://github.com/)

---

> ✨ “Learning Linux is like gaining superpowers — the terminal is your wand!”
