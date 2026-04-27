<img width="884" alt="Screenshot 2025-01-23 at 7 59 52 PM" src="https://github.com/user-attachments/assets/14983237-8b1a-4703-8a5b-d5f0d3e188f9" />

<h1>Azure Virtual Machine Setup</h1>

This tutorial creates the Azure resources for this project. This setup involves creating a resource group, deploying a Windows 10 virtual machine, and a Linux (Ubuntu) virtual machine. Both virtual machines must be connected to the same Virtual Network (VNet) and Subnet. These components will serve as the base infrastructure for future project tasks. <br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Cloud Computing)

<h2>Operating Systems Used </h2>

- Windows 10 (22H2)
- Ubuntu Server 20.04
  
<h2>Deployment Proccess</h2>
<img width="387" alt="Screenshot 2025-01-23 at 8 10 04 PM" src="https://github.com/user-attachments/assets/886eb6b5-b6c1-4b4b-ae98-8415a69a6a3b" />

---

**1. Access Azure Portal**

Sign in to Azure to start creating resources. 

**2. Creating a Resource Group**

<img width="1876" height="924" alt="image" src="https://github.com/user-attachments/assets/74c04b55-8b4e-4667-abc2-a735d8b7ea0d" />
<img width="815" height="469" alt="image" src="https://github.com/user-attachments/assets/f4955556-fd7d-4047-8720-efcb9141c90b" />

In Azure navigate to or search for resource groups and select "Create". For Resource Group configuration you need a name and a region. I named the group "RG-Chatty" and selected the region "West US 2". Click on "Review + Create" then "Create". 

