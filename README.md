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
# 🏗️ Step 1: Setup Domain Controller (DC-1)
Created a VM named DC-1 in Azure using Windows Server 2022

Disabled Windows Firewall for lab testing

Set NIC private IP to static

Added to CyberLab-VNet

# 👨‍💻 Step 2: Setup Client (Client-1)
Created a Windows 10 VM named Client-1 in the same VNet and region

Configured Client-1's DNS to point to DC-1's private IP

Restarted the VM from the Azure Portal to apply DNS changes

# 🌐 Step 3: Verify Connectivity
Successfully pinged DC-1 from Client-1

Virtual Network and Subnet Setup: Created CyberLab-VNet with subnet CyberLab-Subnet
![Screenshot (20)](https://github.com/user-attachments/assets/7ebdef06-b5e9-466c-932f-10098d18d0a9)
--
DC-1 VM Created: Windows Server 2022 configured with static private IP.
![Screenshot (22)](https://github.com/user-attachments/assets/ea4adf63-e4e5-4cda-8b09-04e2289887bd)
--
