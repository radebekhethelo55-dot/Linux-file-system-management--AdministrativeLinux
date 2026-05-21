# Linux-file-system-management--AdministrativeLinux

# 🐧 Linux VM & File System Management

This is a hands-on Linux lab completed as part of my Pre-Degree in Cybersecurity at Eduvos. This lab covers setting up Linux virtual machines and managing the file system entirely from the terminal.

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
| `rsync` | Sync and back up files |

---

## 📋 What Was Done

### Virtual Machine Setup
Created two Linux virtual machines using VirtualBox:
- `linux2030-Zekhethelo`
- `linux2030-KylianMbappe`

Configured each VM with secure passwords and resolved a partitioning issue during setup by manually adjusting VM settings.

### Directory Creation
Created a directory called `wildlife` to organise files:
```bash
mkdir wildlife
```

### File Creation & Editing
Used `nano` to create a text file called `Namibia` and populated it with a list of animals:
```bash
nano Namibia
```

### Sorting & Renaming
Sorted the animal list alphabetically, renamed the file from `Namibia` to `Mzansi`, and verified contents:
```bash
sort Namibia
mv Namibia Mzansi
cat Mzansi
```

### Backup Concepts
Explored backup strategies using `rsync` to sync files to multiple destinations. Key principles applied:
- Log start and end times of every backup
- Verify success/failure in log files
- Maintain redundancy by backing up to at least two locations
- Set up failure alerts using email notifications

```bash
rsync -av /source /local-backup
rsync -av /source /cloud-backup
```

---

## 📚 What I Learned
- How to navigate and manage the Linux file system from the terminal
- Why file organisation and backups matter in a security context
- How `rsync` supports redundancy — a key principle in disaster recovery
- How to read and interpret log files for backup verification

---

## 🎓 About This Lab
Completed as part of the **Higher Certificate in Cybersecurity** at **Eduvos (2025)**.

**Certifications:** Cisco Networking Academy | IBM Cybersecurity Fundamentals

**Currently Studying:** CompTIA Network+ | Security+ | CySA+# 🐧 Linux VM & File System Management

A hands-on Linux lab completed as part of my Higher Certificate in Cybersecurity at Eduvos. This lab covers setting up Linux virtual machines and managing the file system entirely from the terminal.

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
| `rsync` | Sync and back up files |

---

## 📋 What Was Done

### Virtual Machine Setup
Created two Linux virtual machines using VirtualBox:
- `linux2030-Zekhethelo`
- `linux2030-KylianMbappe`

Configured each VM with secure passwords and resolved a partitioning issue during setup by manually adjusting VM settings.

### Directory Creation
Created a directory called `wildlife` to organise files:
```bash
mkdir wildlife
```

### File Creation & Editing
Used `nano` to create a text file called `Namibia` and populated it with a list of animals:
```bash
nano Namibia
```

### Sorting & Renaming
Sorted the animal list alphabetically, renamed the file from `Namibia` to `Mzansi`, and verified contents:
```bash
sort Namibia
mv Namibia Mzansi
cat Mzansi
```

### Backup Concepts
Explored backup strategies using `rsync` to sync files to multiple destinations. Key principles applied:
- Log start and end times of every backup
- Verify success/failure in log files
- Maintain redundancy by backing up to at least two locations
- Set up failure alerts using email notifications

```bash
rsync -av /source /local-backup
rsync -av /source /cloud-backup
```

---

## 📚 What I Learned
- How to navigate and manage the Linux file system from the terminal
- Why file organisation and backups matter in a security context
- How `rsync` supports redundancy — a key principle in disaster recovery
- How to read and interpret log files for backup verification

---

## 🎓 About This Lab
Completed as part of the **Higher Certificate in Cybersecurity** at **Eduvos (2025)**.

**Certifications:** Cisco Networking Academy | IBM Cybersecurity Fundamentals

**Currently Studying:** CompTIA Network+ | Security+ | CySA+
