## 1.Install Git

### Dounload Link:

Go to: https://git-scm.com/download/win

### Installation Steps:

1. Download the installer.

2. Run the installer (keep default settings).

3. After installation, open Git Bash and check version:


sudo apt update
sudo apt install git -y
git --version

-----

## 2.VS Code Installation 

### Download Link:
https://code.visualstudio.com/

---

### Installation Steps:
```bash
sudo apt update
sudo apt install wget gpg -y
wget -qO- https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > packages.microsoft.gpg
sudo install -o root -g root -m 644 packages.microsoft.gpg /usr/share/keyrings/
echo "deb [arch=amd64 signed-by=/usr/share/keyrings/packages.microsoft.gpg] \
https://packages.microsoft.com/repos/vscode stable main" | sudo tee /etc/apt/sources.list.d/vscode.list
sudo apt update
sudo apt install code -y


## VirtualBox / VMware + Kali Linux Installation

-----

### VirtualBox Installation

🔗 Download:  
https://www.virtualbox.org/wiki/Downloads

 For Windows:
- Download **Windows hosts** version
- Install using setup wizard (default options)

 For Linux (Debian/Kali):
``bash
sudo apt update
sudo apt install virtualbox -y


## VMware Workstation Player + Kali Linux VM Setup

-----

### VMware Installation (Linux)

 Download VMware Workstation Player:  
https://www.vmware.com/products/workstation-player.html

#### Steps:
1. Download the latest **VMware Workstation Player** (Free for personal use)
2. Run the installer and follow the setup wizard (default options)
3. Launch **VMware Player** after installation

-----

### Kali Linux VM for VMware

Download Kali Linux VMware Image:  
https://www.kali.org/get-kali/#kali-virtual-machines

####  Steps:
1. Download the Kali Linux `.7z` file (VMware version)
2. Extract it using **7-Zip**
3. Open **VMware Player**
4. Click **Open a Virtual Machine**
5. Select the `.vmx` file from the extracted folder
6. Click **Power on this virtual machine**

 Default login:
- Username: `kali`
- Password: `kali`

---

Kali Linux is now ready inside VMware.

-----

## Importing Kali Linux VM


### Step 1: Download Kali Linux VM

 Official Download Page:  
https://www.kali.org/get-kali/#kali-virtual-machines

#### Choose the correct image:
- For **VirtualBox** → Download `.7z` file under "Kali Linux VirtualBox"
- For **VMware** → Download `.7z` file under "Kali Linux VMware"

---

### Step 2: Extract the File

- Use [7-Zip](https://www.7-zip.org/) or another tool to extract the `.7z` file
- It contains a `.ova` (for VirtualBox) or `.vmx` (for VMware) file

---

### Step 3: Import into VirtualBox

1. Open **VirtualBox**
2. Go to **File > Import Appliance**
3. Select the extracted `.ova` file
4. Click **Next > Import**
5. After import, click **Start** to boot Kali VM

---

### Step 3: Open in VMware

1. Open **VMware Workstation Player**
2. Click **Open a Virtual Machine**
3. Select the extracted `.vmx` file
4. Click **Play Virtual Machine**

---

### Default Credentials

- **Username:** `kali`  
- **Password:** `kali`

---

 You now have Kali Linux running in a virtual environment.

