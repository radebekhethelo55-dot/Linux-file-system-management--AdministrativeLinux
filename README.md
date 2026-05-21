# 🐧 Linux VM & File System Management

This is A hands-on Linux lab completed as part of my Pre-Degree in Cybersecurity at Eduvos. This lab covers setting up Linux virtual machines and managing the file system entirely from the terminal.

---

## 🎯 Objective
Set up Linux virtual machines and practise core file system operations including creating, editing, sorting, renaming, and moving files using the terminal.

---

## 🛠️ Commands Used

| Command | Purpose |
|--------|---------|
| `nano` | Create and edit text files in the terminal |
| `cat` | Display file contents |
| `sort` | Sort content alphabetically |
| `mv` | Move or rename files |
| `mkdir` | Create directories |
| `chmod` | Change file permissions |
| `whoami` | Display current logged in user |
| `ls` | List files in a directory |

---

## 📋 What Was Done

### 1. Virtual Machine Setup
Created two Linux virtual machines using VirtualBox with the following configurations:

**VM 1 — Zekhethelo (linux2030)**

![VM 1 Setup](1.png)

**VM 2 — Kylian Mbappe**

![VM 2 Setup](2.png)

---

### 2. VM Installation & Configuration
VM 1 booted into the Ubuntu installer. User credentials and hostname were configured during setup.

![VM Installation Screen](3.png)

Once booted, the `whoami` command confirmed the logged-in user. An attempt was made to change the admin display name using `sudo chfn` but failed because the user was not in the sudoers file — a key security feature in Linux.

```bash
whoami
sudo chfn -f "Zekhethelo" Administrator
```

![Terminal - whoami and chfn attempt](4.png)

---

### 3. Directory Creation
Navigated the file system and created a `Home` directory and a `WildLife` subdirectory using `mkdir`. Used `ls` to verify they were created successfully.

```bash
mkdir Home
mkdir WildLife
ls
nano Namibia.txt
```

![mkdir and directory creation](5.png)

---

### 4. File Creation with Nano
Used `nano` to create a text file called `Namibia.txt` and populated it with a list of African animals: oryx, springbok, strandjut, puku, sitatunga, topi, oribi, kudu.

![nano editor with Namibia.txt](6.png)

---

### 5. Viewing File Contents
Used `cat` to display the contents of `Namibia.txt` and confirm all animals were saved correctly.

```bash
cat Namibia.txt
```

![cat command output](7.png)

---

### 6. Sorting the File
Used `sort` to sort the animal list alphabetically. Encountered path errors when trying to sort from the wrong directory — learned the importance of being in the correct working directory.

```bash
sort Namibia.txt
```

![sort command output](8.png)

---

### 7. Renaming & Verifying with cat
Renamed `Namibia.txt` to `Mzansi.txt` using `mv`, then used `cat` to verify the contents were preserved after renaming.

```bash
mv Namibia.txt Mzansi.txt
cat Mzansi.txt
```

![mv rename and cat verification](9.png)

---

### 8. Moving to Backup Directory (Attempted)
Attempted to move `Mzansi.txt` to a backup directory. Multiple errors occurred due to incorrect paths and directory names. Eventually successfully renamed the file to `Backup/Mzansi.txt`.

```bash
mkdir -p backup
mv Mzansi.txt Backup/
```

![Backup directory move attempts](10.png)

---

### 9. File Permissions with chmod (Attempted)
Attempted to change file permissions using `chmod 600` on the Backup directory. Encountered errors due to using placeholder paths instead of actual paths — a valuable lesson in Linux path syntax.

```bash
chmod 600 /absolute/path/to/Backup
```

![chmod permission attempts](11.png)

---

## 📚 What I Learned
- How to set up and configure Linux virtual machines from scratch using VirtualBox
- How to navigate the Linux file system entirely from the terminal
- How `nano`, `cat`, `sort`, and `mv` work together for file management
- Why correct file paths are critical when moving or accessing files
- How `chmod` controls file permissions and what the numbers mean (e.g. 600 = owner read/write only)
- That the sudoers file controls who has admin privileges — a core Linux security concept
- That errors and troubleshooting are a normal and valuable part of working in Linux 💪

---

## 🎓 About This Lab
Completed as part of the **Pre-Degree Cybersecurity(2025)** 

**Certifications:** Cisco Networking Academy | IBM Cybersecurity Fundamentals

**Currently Studying:** CompTIA Network+ | Security+ | CySA+
