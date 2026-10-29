Student Information
Name: Christine Nakyanzi
Batch: B084
Task: WK1-PM1 Lab Setup
Instructor: Waqas Karim CCE
Date: 27 October 2026
lAB OBJECTIVE
The objective of this project was to build and configure a cybersecurity laboratory environment using VirtualBox and Kali Linux for safe penetration testing practice and cybersecurity training.

LAB DETIALS
✅Hypervisor: VirtualBox (Latest Version)
✅Network Type: NAT Network
✅Operating System: Kali Linux-2026.2-virtualbox-amd64.
✅Internet Connectivity: Successfully Configured
✅Network Configuration: Private Lab E

INSTALLATION METHOD
I downloaded the Kali Linux VirtualBox image from the official Kali Linux website and extracted the downloaded file. After installing VirtualBox, I imported the Kali Linux virtual machine and started it successfully. Once the operating system finished booting, the environment was ready for login and configuration.

CONFIQURATION STEPS
1. Create NAT Network
Navigation:

File → Tools → Network Manager → NAT Networks → Create
Configuration:

Created a NAT Network
Enabled DHCP
Verified network availability
2. Import Kali Linux Virtual Machine
Imported the Kali Linux VirtualBox image and configured the network adapter.

Network Settings:

Settings → Network → Adapter 1
Attached To: NAT Network
Promiscuous Mode: Allow All
3. Enable Virtual Machine Features
Enabled the following features:

Shared Clipboard: Bidirectional
Drag and Drop: Bidirectional
Installed VirtualBox Guest Additions to improve system integration and usability.

4. Configure Network Settings
Configured network settings inside Kali Linux and verified connectivity using network diagnostic commands.

5. Create Snapshot
Created a snapshot of the completed setup for future recovery and lab activities.

Snapshot Name:My First kali project

CHALLENGES  ENCOUNTERED AND SOLUTIONS

CHALLENGE 1: Network Connectivity Issues
While working on the lab, the Kali Linux virtual machine would occasionally disconnect from the network. When this happened, internet access would stop working, which interrupted updates, downloads, and testing activities.
🚨 CHALLENGES ENCOUNTERED AND SOLUTIONS

🔴 CHALLENGE 1: NETWORK CONNECTIVITY ISSUES
While working on the lab, the Kali Linux virtual machine would occasionally disconnect from the network. This caused internet access to stop working and interrupted downloads, updates, and testing activities.

✅ SOLUTION

Checked the VirtualBox network settings.
Confirmed that the virtual machine was connected to the correct NAT Network.
Restarted the network adapter.
Verified the network configuration.
Retested connectivity using ping commands.
After correcting the configuration, the connection became stable and internet access was restored.

🔴 CHALLENGE 2: NETWORK CONFIGURATION NOT PERSISTING AFTER REBOOT
After restarting the virtual machine, the internet connection would sometimes fail to reconnect automatically.

✅ SOLUTION
To restore internet connectivity, I used the following command:

sudo nmcli connection modify "Wired connection 1" ipv4.dad-timeout 0
Steps performed:

Opened the terminal.
Entered the command above.
Pressed Enter.
Entered my password when prompted.
The network connection was restored successfully.

✅ VERIFICATION

PROOF SCREEN SHOTS.

✅ NAT NETWORK.png

✅ ip-a.png

✅ vm-settings-network.png

✅ ping-8.8.8.8.png

✅ snapshot.png

📚 LESSONS LEARNED
During this lab, I gained hands-on experience with:

✅ VirtualBox installation and configuration

✅ NAT network configuration

✅ Kali Linux deployment and management

✅ Virtual machine networking

✅ Troubleshooting network connectivity issues

✅ Internet connectivity verification

✅ Creating and managing snapshots

✅ Problem-solving in virtualized environments

✅ Cybersecurity lab setup best practices

CONCLUSION.
The cybersecurity lab was successfully created and configured using VirtualBox and Kali Linux. The virtual machine was able to access the internet, the required settings were configured correctly, and a recovery snapshot was created. This lab provided valuable practical experience in virtualisation, networking, and cybersecurity fundamentals.