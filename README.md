# VPN Setup in a Virtual Machine — Step-by-Step Guide

**A practical guide** to set up and test a VPN inside a Windows 10 virtual machine on Azure.  
This guide demonstrates how to install Proton VPN, connect, and verify your VPN connection.

---

## 🚩 What This Guide Is For
**Goal:** Learn to set up a VPN inside a VM, connect to a server, and verify IP masking.  
**Target audience:** Anyone learning IT, virtual networking, or experimenting with VPNs.<br>
**Estimated time:** 30–60 minutes

---

## 🛠 Prerequisites
- Microsoft Azure account  
- Ability to create a Resource Group and deploy a Windows 10 VM  
- Remote Desktop access (RDP) to the VM  
- Internet connection on both host and VM  
- Proton VPN account (free version works fine)  

---

## 📋 Environments and Technologies Used
- **VPN:** Proton VPN  
- **Cloud Platform:** Microsoft Azure (Virtual Machines/Compute)  
- **Remote Access:** RDP  
- **Operating System:** Windows 10 (21H2)  

---

## ✅ Installation & Setup Steps

### 1 — Deploy a Virtual Machine
1. Log into **Azure Portal**.  
2. Create a **Resource Group** for your project.  
3. Deploy a **Windows 10 Virtual Machine** inside this resource group.  
4. Once the VM is ready, connect using **Remote Desktop Protocol (RDP)**.

---

### 2 — Check Your Current IP
1. Inside the VM, open a web browser.  
2. Go to [https://whatismyipaddress.com/](https://whatismyipaddress.com/)  
3. Record the IP address somewhere (Notepad or on paper) for later reference.

---

### 3 — Download and Install Proton VPN
1. On your personal computer, sign up for a free Proton VPN account: [https://account.protonvpn.com/signup](https://account.protonvpn.com/signup?plan=free&language=en)  
2. Inside the VM, download the Proton VPN client: [https://account.protonvpn.com/login](https://account.protonvpn.com/login)  
3. Install the client following the on-screen instructions.

---

### 4 — Connect to the VPN
1. Open the **Proton VPN client** inside the VM.  
2. Log in with the credentials from your Proton VPN account.  
3. Click **Quick Connect** to automatically connect to the best available VPN server.  
4. Your internet traffic is now encrypted and your IP address is masked.

---

### 5 — Verify the VPN Connection
1. Revisit [https://whatismyipaddress.com/](https://whatismyipaddress.com/) in the VM.  
2. Observe the IP address — it should now reflect the VPN server location.  
3. Note the changes to confirm your connection is active and working correctly.

---

### 6 — Optional: Test Internet Access
- Open a web browser and try accessing websites.  
- Ensure there is no connection loss or blocked content.  
- Disconnect/reconnect the VPN to test stability and speed.

---

### ✅ Notes & Tips
- Always record your original IP before connecting to a VPN for testing purposes.  
- Use the VM for safe experimentation; your host PC’s IP will remain private.  
- This setup is useful for testing VPN configurations, remote work simulations, or privacy labs.
