# NETWORKWALKS-IDOWU-SAMUEL-JESUTOFUNMI-B084-WK1-PM1-CYBERSECURITY-LAB-SETUP
Cybersecurity lab setup

Step 1. Install 7-Zip
I successfully installed 7-Zip to extract the Kali Linux virtual-machine

Step 2. Install VirtualBox
VirtualBox was successfully installed.

Step 3. Create the NAT Network
I created a NAT Network successfully in VirtualBox.

Configuration: Network Name: NatNetwork IPv4 Prefix: 10.0.0.0/24 DHCP: Enabled IPv6: Disabled

selected a NAT Network to grant the virtual machines outbound network access while allowing them to communicate with each other. This enables future attacker and target VMs to interact inside the lab.


Step 4. Import Kali Linux
The Kali Linux virtual machine was downloaded from the official Kali Linux website and imported into VirtualBox.


A workaround used during this lab was:

sudo nmcli connection modify "Wired connection 1" ipv4.dad-timeout 0
The network connection was then restarted/rebooted and connectivity was tested again.

challenges 
Virtualization Error
MY VM initially couldn't start because the virtualization was disabled on BIOS settings 

I was able to resolve this issue by:

Restarting my PC.
Entering BIOS/UEFI settings.
Enabling hardware virtualization technology.
Saving the configuration.
Restarting the computer.
Starting the Kali VM again.
After enabling virtualization, the VM started successfully and I was able to complete the setup.
