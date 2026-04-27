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

<h2>1. Access Azure Portal</h2>

Sign in to Azure to start creating resources. 

<h2>2. Creating a Resource Group</h2>

<img width="1876" height="924" alt="image" src="https://github.com/user-attachments/assets/74c04b55-8b4e-4667-abc2-a735d8b7ea0d" />
<img width="815" height="469" alt="image" src="https://github.com/user-attachments/assets/f4955556-fd7d-4047-8720-efcb9141c90b" />

In Azure navigate to or search for resource groups and select "Create". For Resource Group configuration you need a name and a region. I named the group "RG-Chatty" and selected the region "West US 2". Click on "Review + Create" then "Create". 

<h2>3. Creating a Windows 10 Virtual Machine</h2>

<img width="1864" height="875" alt="image" src="https://github.com/user-attachments/assets/9decf61c-2536-493c-a88f-7da5e9c9ff5d" />

Navigate to or search for Virtual Machines (VMs) and click on "Create". 

<img width="951" height="869" alt="image" src="https://github.com/user-attachments/assets/c9ab7867-2aef-4774-a7e0-2d5123d6a43b" />
<img width="799" height="384" alt="image" src="https://github.com/user-attachments/assets/6104dbe1-4514-4447-8bb6-210b881b569b" />

In the Virtual Machine creation make sure the following details are selected:
   - Resource Group: "RG-Chatty"
   - Region: West US 2
   - Virtual Machine Name: "Windows-VM" (Can be something different if you want)
   - Image: Windows 10 Enterprise, version 22H2 -  x64 Gen2
   - Size: Standard_L2as_v4 - 2 vcpus, 16 GiB memory
   - Administrator Account:
       Username: labuser
       Password: Cyberlab123!

<img width="1874" height="873" alt="image" src="https://github.com/user-attachments/assets/fc07fbf5-1e44-44a4-9c62-b73e940e7c86" />
<img width="457" height="152" alt="image" src="https://github.com/user-attachments/assets/35b3396f-1ac5-4f11-8077-56e1ff47b68a" />

Navigate to the Networking tab of the Virtual Machine. Create a new Virtual network. I named mine "Lab-Vnet" and click OK. Select "Review + Create" and "Create". 

The Virtual Network is important because it allows Virtual Machines on the same network to communicate securely over the same internal network and have proper network interactions.

<h2>4. Creating a Linux Virtual Machine</h2>

Navigate to or search for Virtual Machines (VMs) and click on "Create". 

<img width="1379" height="891" alt="image" src="https://github.com/user-attachments/assets/e95b6c0f-3ce8-4554-b9ad-a6dc378463ec" />
<img width="1380" height="676" alt="image" src="https://github.com/user-attachments/assets/c88d29f5-4d3b-42bd-b348-664042cee7bb" />

In the Virtual Machine creation make sure the following details are selected:
   - Resource Group: "RG-Chatty"
   - Region: West US 2
   - Virtual Machine Name: "Linux-VM" (Can be something different if you want)
   - Image: Ubuntu Server 24.04 LTS - x64 Gen2
   - Size: Standard_L2as_v4 - 2 vcpus, 16 GiB memory
   - Administrator Account:
       Username: labuser
       Password: Cyberlab123!

<img width="1157" height="644" alt="image" src="https://github.com/user-attachments/assets/01f3427d-2ae4-4b63-8646-8ce102415869" />

Verify in the Networking tab that the proper Virtual Network is selected. I selected my previously created "Lab-Vnet" because thats where my windows virtual machine is at so they can be on the same network to communicate securely. Navigate to "Review + Create" and "Create". 

<h2>End of Project</h2>
<img width="1865" height="580" alt="image" src="https://github.com/user-attachments/assets/72df3074-79a4-4fdc-81df-462c4eefb0b8" />

Verify that both Virtual Machines were created properly within the same Resource Group and Virtual Network. The goal of this tutorial was core Azure infrastructure needed for the next project of this section. The main components used during setup were Virtual Machines, a Resource Group, and a Virtual Network. The setup creates an enviornment for the Virtual Machines to communicate on. 







     
