# WK1-PM1 Cybersecurity Lab Setup

## Intern Details

Name: Lubanzi Fihla

Program:
NetworkWalks Cybersecurity Internship

## Objective

Build a Cybersecurity Lab using VirtualBox and Kali Linux.

## Lab Requirements

- VirtualBox Installed
- NAT Network 10.0.0.0/24
- Kali Linux Installed
- Static IP 10.0.0.2/24
- Internet Connectivity
- Shared Clipboard Enabled
- Shared Folder Enabled

## Steps Performed

### Step 1
Installed VirtualBox.

### Step 2
Created NAT Network 10.0.0.0/24.

### Step 3
Imported Kali Linux VM.

### Step 4
Configured network adapter to NAT Network.

### Step 5
Assigned static IP 10.0.0.2/24.

### Step 6
Verified internet connectivity.

### Step 7
Enabled clipboard and drag-and-drop.

### Step 8
Configured shared folder.

### Step 9
Created VM snapshot.

## Screenshots

### NAT Network Setup

screenshots/01-nat-network.png

### Kali Settings

![Settings](screenshots/02-kali-settings.png)

s

![IP](screens3-ip-address.png

### Ping Test

screenshots/04-ping-test.png

## Lessons Learned

- VirtualBox Networking
- Kali Linux Configuration
- Static IP Addressing
- Virtual Machine Management
- Snapshot Management

## Troubleshooting

Issue:
Kali Linux had no internet access.

Solution:
Executed:

sudo nmcli connection modify "Wired connection 1" ipv4.dad-timeout 0

sudo nmcli connection down "Wired connection 1"

sudo nmcli connection up "Wired connection 1"

Internet connectivity was restored.
