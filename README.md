DAY 02

# Kali Linux Installation on VirtualBox

This guide shows you how to install Kali Linux on Oracle VirtualBox step by step.

---

## Requirements

- Oracle VM VirtualBox (download: https://www.virtualbox.org/)
- Kali Linux ISO file (download: https://www.kali.org/get-kali/)
- Minimum 4 GB RAM, 20 GB disk space

---

## Steps to Install

### 1. Download Files

- Download and install VirtualBox
- Download the Kali Linux ISO image

### 2. Create a New Virtual Machine

- Open VirtualBox → Click **New**
- Name: `Kali Linux`
- Type: `Linux`
- Version: `Debian (64-bit)`
- Memory: at least **4 GB (4096 MB)**
- Create a virtual hard disk now → **VDI**, **Dynamically allocated**, **20 GB or more**

### 3. Attach Kali ISO

- Go to **Settings → Storage**
- Under Controller: IDE, click **Empty**
- On the right side, click the disk icon → **Choose a disk file**
- Select your downloaded Kali ISO

### 4. Start the VM and Install Kali

- Click **Start**
- Choose **Graphical install**
- Follow setup: Language, location, keyboard
- Set username and password
- Use entire disk for installation
- Select Yes to install GRUB bootloader → Choose `/dev/sda`

### 5. First Boot

- After installation completes, unmount the ISO from Storage
- Start the VM
- Login with the username and password you created

---

## (Optional) Install Guest Additions

To enable full screen, drag & drop, shared clipboard:

```bash
