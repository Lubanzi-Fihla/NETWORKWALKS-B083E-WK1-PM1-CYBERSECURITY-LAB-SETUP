# WK1-PM1 Cybersecurity Lab Setup

## Intern Details

**Name:** Lubanzi Fihla

**Program:** NetworkWalks Cybersecurity Internship

---

## Objective

Build a Cybersecurity Lab using Oracle VirtualBox and Kali Linux.

---

## Lab Requirements

- VirtualBox Installed
- NAT Network (10.0.0.0/24)
- Kali Linux Installed
- Static IP Address (10.0.0.2/24)
- Internet Connectivity
- Shared Clipboard Enabled
- Shared Folder Enabled

---

## Steps Performed

### Step 1
Installed Oracle VirtualBox.

### Step 2
Created NAT Network `10.0.0.0/24`.

### Step 3
Imported Kali Linux Virtual Machine.

### Step 4
Configured Network Adapter to CyberLab NAT Network.

### Step 5
Assigned Static IP Address:

```text
10.0.0.2/24
Gateway: 10.0.0.1
```

### Step 6
Verified Internet Connectivity.

### Step 7
Enabled Shared Clipboard and Drag-and-Drop.

### Step 8
Configured Shared Folder.

### Step 9
Created Virtual Machine Snapshot.

---

## Screenshots

### Kali Linux Desktop Running Successfully
![Kali Desktop](screenshots/01-Kali%20desktop%20runningpng

### NAT Network Configuration
![NAT Network](screenshots/02-NAT%erLab.png

### Static IP Configuration
![Static IP](screenshots/03-ip%20a%20displaying%2010.0.0.2%20

### Default Gateway Connectivity Test
![Gateway Ping](screenshots/04-Ping%20Default### Internet Connectivity Test (8.8.8.8)
![Ping 8.8.8.8](screenshots/05-ping%208.8.8.8%20successful.png)

n Test
![Ping Google](screenshots/06-ping%20googlehared Folder Configuration
![Shared Folder](screenshots/07-Shared%20irtualBox VM Settings
![VM Settings](screenshots/08-VirtualBoxs.png

---

## Lessons Learned

- VirtualBox Network Configuration
- Kali Linux Installation
- Static IP Configuration
- NAT Networking
- DNS Troubleshooting
- Virtual Machine Management
- Snapshot Management

---

## Troubleshooting

### Problem

Kali Linux could access IP addresses but could not resolve domain names.

```bash
ping google.com
Temporary failure in name resolution
```

### Root Cause

The DNS configuration file `/etc/resolv.conf` was missing.

### Solution

Created the DNS configuration file and added:

```text
nameserver 8.8.8.8
nameserver 1.1.1.1
```

### Result

- Gateway Connectivity: Successful 
- Ping 8.8.8.8: Successful 
- Ping google.com: Successful 

---

## Conclusion

The Cybersecurity Lab was successfully configured using VirtualBox and Kali Linux. The environment now supports static addressing, Internet access, DNS resolution, shared folders, and virtual machine management.
