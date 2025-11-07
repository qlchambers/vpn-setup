# VPN Setup in a Virtual Machine — Step-by-Step Guide

A guide that teaches you how to set up and test a VPN inside a Windows 10 virtual machine on Azure.  
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
3. Create a Windows 10 Virtual Machine inside this resource group.  <img width="1444" height="296" alt="image" src="https://github.com/user-attachments/assets/32d93778-8e03-448c-aeaf-85d0e951e2c4" />
4. Once the VM is ready, connect using Remote Desktop Protocol (RDP).<br>
   <img width="403" height="241" alt="image" src="https://github.com/user-attachments/assets/0a06f1c4-5259-441a-b907-be4bcbc5710c" />





### 2 — Check Your Current IP
1. Once you're the VM, open up a web browser.  
2. Go to [https://whatismyipaddress.com/](https://whatismyipaddress.com/)  
3. Write down the IP address somewhere (Notepad or on paper) to come back to later.
   


### 3 — Download and Install Proton VPN
1. On your PC, sign up for a free Proton VPN account: [https://account.protonvpn.com/signup](https://account.protonvpn.com/signup?plan=free&language=en)  
2. Inside the Azure VM, download the Proton VPN application: [https://account.protonvpn.com/login](https://account.protonvpn.com/login)  
3. Install the application by following the on screen instructions.<br>
<img width="586" height="458" alt="image" src="https://github.com/user-attachments/assets/9bccd4f4-2e57-4974-8b3e-9365b9598a57" />



### 4 — Connect to the VPN
1. Open the Proton VPN application inside the VM.  
2. Log in with the same password and username from your Proton VPN account.  
3. Click Connect to automatically connect to the best available VPN server. 
4. Your internet traffic is now encrypted and your IP address is masked.<br>
   <img width="435" height="199" alt="image" src="https://github.com/user-attachments/assets/b1a139b7-9401-4384-b28e-ada99e2c04e1" />
   



### 5 — Verify the VPN Connection
1. Go back to [https://whatismyipaddress.com/](https://whatismyipaddress.com/) in the VM.  
2. Look at your new IP Address, it should now be associated with the same location as the VPN server.  
3. Make sure to confirm your connection is active and working correctly.<br> <img width="1195" height="480" alt="image" src="https://github.com/user-attachments/assets/c856266c-3e21-40e5-88dc-da641e2acbe6" />


### 6 — Optional: Test Internet Access
- Open a web browser and try accessing websites.  
- Make sure that there is no connection loss or blocked content.  
- Disconnect/reconnect the VPN to test connectivity and speed.


### ✅ Notes & Tips
- Record your original IP BEFORE connecting to a VPN for testing purposes.  
- The VM has its own separate IP, so your host PC stays hidden and safe online.
- This setup is useful for testing VPN configurations and remote work.
