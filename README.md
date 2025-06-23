# 🖥️ Azure Active Directory Lab Setup
This project demonstrates how to set up a simple Windows Server Active Directory lab in Microsoft Azure. The lab includes a Domain Controller (DC-1) and a Windows 10 Client (Client-1) connected via the same virtual network. It’s ideal for learning domain environments, group policy, and Windows network services.

# 🧱 Lab Infrastructure
Resource Group: CyberLab-RG

Virtual Network: CyberLab-VNet with Subnet CyberLab-Subnet

DC-1 (Domain Controller)

OS: Windows Server 2022

Username: labuser

IP: Static Private IP

Role: Domain Controller

Client-1

OS: Windows 10

Username: labuser

Configured with DC-1 as its DNS server

# 🛠️ Configuration Steps
🏗️ Step 1: Setup Domain Controller (DC-1)
Created a VM named DC-1 in Azure using Windows Server 2022

Disabled Windows Firewall for lab testing

Set NIC private IP to static

Added to CyberLab-VNet

👨‍💻 Step 2: Setup Client (Client-1)
Created a Windows 10 VM named Client-1 in the same VNet and region

Configured Client-1's DNS to point to DC-1's private IP

Restarted the VM from the Azure Portal to apply DNS changes

🌐 Step 3: Verify Connectivity
Successfully pinged DC-1 from Client-1

Verified DNS setting in ipconfig /all showing DC-1 as the DNS Server

