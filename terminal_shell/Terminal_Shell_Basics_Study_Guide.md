# 🧠 Terminal / Shell Basics Study Guide

This guide introduces essential terminal commands for navigating and managing your system via the command line. It assumes a Unix-style shell (macOS Terminal, Linux, PowerShell Core, or Git Bash). Where necessary, Windows-specific notes are called out.

---

## 📁 1. File and Directory Navigation

### Current Directory
```bash
pwd
```
Prints the current directory path.

### List Files
```bash
ls
```
List files and folders in the current directory.

> 🪟 **Windows CMD** uses `dir`

### Change Directory
```bash
cd foldername
```
Move into a directory.

```bash
cd ..
```
Go up one directory level.

---

## 📂 2. File and Directory Operations

### Create a File
```bash
touch filename.txt
```
Creates a new empty file.

> 🪟 PowerShell alternative:
```powershell
New-Item filename.txt
```

### Create a Directory
```bash
mkdir newfolder
```

### Delete a File
```bash
rm filename.txt
```

> 🪟 PowerShell alternative:
```powershell
Remove-Item filename.txt
```

### Delete a Directory
```bash
rm -r foldername
```

---

## 📝 3. Viewing and Editing Files

### Show File Contents
```bash
cat filename.txt
```

### Open File in Editor (e.g., nano)
```bash
nano filename.txt
```

> 🪟 PowerShell may require `notepad filename.txt` or install `nano`

---

## ⚙️ 4. System Utilities

### Clear the Terminal
```bash
clear
```

> 🪟 CMD uses `cls`

### Command History
```bash
history
```

### Repeat Last Command
```bash
!!
```

---

## 🔍 5. Searching and Pipes

### Search Inside a File
```bash
grep "text" filename.txt
```

> 🪟 PowerShell equivalent:
```powershell
Select-String -Path filename.txt -Pattern "text"
```

### Combine Commands (Pipes)
```bash
cat file.txt | grep "term"
```

---

## 🎯 6. Permissions (Unix/Mac)

### Make a File Executable
```bash
chmod +x script.sh
```

> 🪟 Not usually needed in Windows

---

## 🧪 7. Try It Yourself

```bash
mkdir demo
cd demo
touch hello.txt
echo "Hello, world!" > hello.txt
cat hello.txt
```

---

## ✅ Tips

- Use `Tab` to autocomplete file/folder names.
- Use `Ctrl+C` to stop a running command.
- Use `Ctrl+L` to clear the screen (Unix).
- Always check your current directory with `pwd`.

---

This guide gives you the essentials for working in the terminal across macOS, Linux, and modern Windows setups (PowerShell, Git Bash, WSL).

