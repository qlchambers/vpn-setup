# VPN Setup in a Virtual Machine — Step-by-Step Guide

A practical guide to set up and test a VPN inside a Windows 10 virtual machine on Azure.  
This guide demonstrates how to install Proton VPN, connect, and verify your VPN connection.


## 🚩 What This Guide Is For
Goal: Learn to set up a VPN inside a VM, connect to a server, and verify that the IP returns encrypted.<br>Target audience: Anyone learning IT, virtual networking, or experimenting with VPNs.<br>
Estimated time: 30–60 minutes.



## 🛠 Prerequisites
- Microsoft Azure account  
- Able to create a Resource Group and deploy a Windows 10 VM  
- Remote Desktop access (RDP) to the VM  
- Internet connection on both host and VM  
- Proton VPN account (the free version will also work)  


## 📋 Environments and Technologies Used
- VPN: Proton VPN  
  Cloud Platform: Microsoft Azure (Virtual Machines)  
- Remote Access: RDP  
- Operating System: Windows 10


## ✅ Installation & Setup Steps

### 1 — Deploy a Virtual Machine
1. Log into Azure Portal.  
2. Create a Resource Group.  
3. Create a Windows 10 Virtual Machine inside this resource group.  
4. Once the VM is ready, connect using Remote Desktop Protocol (RDP).


### 2 — Check Your Current IP
1. Once you're the VM, open up a web browser.  
2. Go to [https://whatismyipaddress.com/](https://whatismyipaddress.com/)  
3. Write down the IP address somewhere (Notepad or on paper) to come back to later.


### 3 — Download and Install Proton VPN
1. On your PC, sign up for a free Proton VPN account: [https://account.protonvpn.com/signup](https://account.protonvpn.com/signup?plan=free&language=en)  
2. Inside the Azure VM, download the Proton VPN application: [https://account.protonvpn.com/login](https://account.protonvpn.com/login)  
3. Install the application by following the on screen instructions.


### 4 — Connect to the VPN
1. Open the Proton VPN application inside the VM.  
2. Log in with the same password and username from your Proton VPN account.  
3. Click Quick Connect to automatically connect to the best available VPN server.  
4. Your internet traffic is now encrypted and your IP address is masked.


### 5 — Verify the VPN Connection
1. Go back to [https://whatismyipaddress.com/](https://whatismyipaddress.com/) in the VM.  
2. Look at your new IP Address, it should now be associated with the same location as the VPN server.  
3. Make sure to confirm your connection is active and working correctly.


### 6 — Optional: Test Internet Access
- Open a web browser and try accessing websites.  
- Make sure that there is no connection loss or blocked content.  
- Disconnect/reconnect the VPN to test connectivity and speed.


### ✅ Notes & Tips
- Record your original IP BEFORE connecting to a VPN for testing purposes.  
- The VM has its own separate IP, so your host PC stays hidden and safe online.
- This setup is useful for testing VPN configurations and remote work.
