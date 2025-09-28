# Azure VM Deployment and configuration lab
In this lab, I demonstrate how to deploy and configure a Virtual Machine (VM) using the Microsoft Azure portal. I walk through the full setup process—from creating the VM to configuring availability zones, security settings, and network components.

I also attach and configure additional disks, manage inbound and outbound network access, and ensure that associated resources like public IPs and network interfaces (NICs) are properly cleaned up when the VM is deleted. This lab showcases my ability to manage Azure compute resources with precision and best practices.

## 🎯 Lab Objectives – Azure Virtual Machine Deployment
- I explored the importance of deploying virtual machines in Microsoft Azure to support scalable and secure cloud infrastructure.

- I learned how to create a VM using the Azure portal, configuring key settings such as availability zones, operating system, and authentication methods.

- I gained hands-on experience attaching and configuring additional disks to enhance storage performance and flexibility.

- I managed network access by configuring inbound and outbound rules, ensuring secure connectivity to and from the VM.

- I verified that associated resources—such as public IP addresses and network interfaces (NICs)are properly removed when the VM is deleted, maintaining clean resource hygiene.


## 📸 Screenshots
###  Step 1: Click Create a resource  
_Selected “Create a resource” from the Azure portal homepage to begin provisioning a new cloud service or infrastructure component._

 ![Click Create a resource ](screenshot/Create-Resrourece%20tab%20VM%20Deployment.png)

### Step 2: Click the Windows Server 2019 Datacenter button  
_Selected the “Windows Server 2019 Datacenter” image from the Azure Marketplace to begin provisioning a new virtual machine._

![Click the Windows ](screenshot/Choosing%20OS-Windows%20Server%202009%20Datacenter%20%20VM%20Deployment.png)

### Step 3: Click the Resource group dropdown  
_Selected the resource group dropdown to choose or create a logical container for the new virtual machine._

 ![VM Creation – Resources Group Tadropdown ](screenshot/Resources-Group%20ProGrp%20%20VM%20Deployment.png)  

### Step 4: Select the Virtual machine name field  
_Clicked into the “Virtual machine name” field to define a unique identifier for the new VM being provisioned._

 ![VM Creation - Select Virtual Machine Name Field ](screenshot/Select%20Virtual%20Machine%20Name%20%20VM%20Deployment.png)

### Step 5: Type SRV01 and press Enter  
_Entered `SRV01` as the virtual machine name to uniquely identify the new deployment within the selected resource group._

 ![Type SRV01 and press Enter ](screenshot/Type%20SRV01%20for%20VM%20name%20.png) 

### Step 6: Click the Availability options dropdown  
_Selected the availability configuration to define redundancy and uptime settings for the SRV01 virtual machine._

 ![Click the Availability options dropdown ](screenshot/Availability%20option-%20Click%20dropdown%20%20VM%20Deployment.png)

### Step 7: Choose Availability Zone  
_Selected “Availability Zone” from the redundancy options to enhance fault tolerance and ensure high availability for virtual machine `SRV01`._

 ![Choose Availability Zone ](screenshot/Select%20Availabilty%20Zone%20from%20list%20%20VM%20Deployment.png)

### Step 8: Click the Availability zone dropdown  
_Selected a specific Availability Zone to deploy `SRV01` into a physically isolated datacenter within East US, enhancing resilience and uptime._

![Click the Availability zone dropdown ](screenshot/availability%20zone-%20dropdown%20to%20see%20list%20%20VM%20Deployment.png)

### Step 9: Click the Availability zone dropdown  
_Selected zone “1” from the Availability Zone list to physically isolate `SRV01` within East US for enhanced fault tolerance and service continuity._

![Choose the Availability zone 1 ](screenshot/Click%20form%20list%20the%20availability%20Zone%201%20%20VM%20Deployment.png)

### Step 10: Click Security type dropdown  
_Selected the security type for `SRV01` to define baseline protections and compatibility with trusted launch or standard deployment options. This step helps shape the VM’s security posture — a key decision for compliance and workload integrity_

![Click Security type dropdown](screenshot/Security%20type%20click%20dorpdown%20%20VM%20Deployment.png)

### Step 11: Select Standard  
_Opted for “Standard” security to apply baseline protections for virtual machine `SRV01`, ensuring compatibility across trusted hardware and common workloads. This step balances security and flexibility — perfect for general-purpose deployments._

![Select Standard](screenshot/Security%20type-%20Select%20standard%20%20VM%20Deployment.png)

### Step 12: Click Size dropdown  
_Opened the VM size selector to choose the appropriate CPU and memory configuration for `SRV01`, balancing performance needs with cost efficiency. This step locks in the compute profile for your deployment — a key decision for lab performance and budget control_

![Click Size dropdown](screenshot/Size%20dorpwond%20to%20choose%20form%20list%20%20VM%20Deployment.png)

### Step 13: Select Standard_D4s_v3  
_Chosen the `Standard_D4s_v3` VM size to allocate 4 vCPUs and 16 GiB of memory to `SRV01`, balancing performance requirements with budget considerations. This step locks in a solid compute profile — ideal for heavier workloads or multi-role lab setups._

![Select Standard_D4s_v3 ](screenshot/Size%20select%20Standard.png)

### Step 14: Click the Username field  
_Clicked into the “Username” field to begin setting up the administrator account for managing virtual machine `SRV01`. This step initiates secure access setup — a key move for remote management and control._

![Click the Username field - Administrator Field](screenshot/Adminitrator%20account-%20file%20username%20and%20password%20field%20%20VM%20Deployment.png)

### Step 15: Type vmadmin and press Enter  
_Entered `vmadmin` as the administrator username for virtual machine `SRV01`, establishing secure access credentials for remote management. This step sets the foundation for authenticated control — a key part of your VM deployment flow._

![Type vmadmin and press Enter - Adminitrator](screenshot/Adminitrator%20accoun-%20username%20fill%20with%20vmadmin%20%20VM%20Deployment.png)

### Step 16: Click Select inbound ports dropdown  
_Opened the inbound ports dropdown during VM creation to configure public access rules such as RDP (port 3389) or HTTP (port 80). This step is key for enabling secure remote access or web traffic — perfect for setting up connectivity during deployment._

![Click Select inbound ports dropdown](screenshot/Select%20inbound%20ports%20dropdown%20%20VM%20Deployment.png)

### Step 17: Select RDP (3389) inbound port  
_Opened the inbound ports dropdown during VM creation and selected **RDP (3389)** to enable secure Remote Desktop access to the Windows virtual machine. This step is essential for remote administration — perfect for labs, testing, or production environments._

![Select RDP (3389) inbound port  ](screenshot/Inbound%20ports-%20select%20RDP(3389)%20%20VM%20Deployment.png)

### Step 18: Click Next: Disks  
_Advanced to the **Disks** configuration tab during VM creation to define OS disk type, attach data disks, and set encryption options before deployment. This step transitions you into storage setup — perfect for customizing performance, redundancy, or backup strategy._

[Click Next: Disks](screenshot/Disk-%20Click%20Next%20Disks%20%20VM%20Deployment.png)

### Step 19: Click OS disk size dropdown  
_Selected the OS disk size dropdown during VM creation to choose between **image default 127GiB**  balancing performance, cost, and redundancy. This step is key for tailoring disk performance to your workload — whether you're optimizing for speed or budget_

[Disk Attachment - Disk OS](screenshot/OS%20disk%20size%20click%20dropdown%20%20VM%20Deployment.png)

### Step 20: Select default OS disk size (127 GiB)  
_Selected the default OS disk size of **127 GiB** during VM creation, which matches the base image size (Windows Server 2019 Datacenter). This disk accommodates the OS, system updates, and essential runtime dependencies. For workloads requiring additional storage, data disks can be attached separately._

![Disk Attachment - Choose Default OS](screenshot/OS%20disk%20size%20click%20defualt%20%20%20VM%20Deployment.png)

### Step 21: Click OS disk type dropdown  
_Selected the OS disk type dropdown during VM creation to choose between storage tiers like Premium SSD, Standard SSD, Standard HDD, or Ultra Disk — balancing performance, durability, and cost for the operating system volume._

![Disk Attachment - Diskt type - Dropdown List](screenshot/OS%20disk%20type%20click%20dropdown%20VM%20Deployment.png)

### Step 22: Select Standard HDD OS disk type  
_Chosen “Standard HDD” as the OS disk type during VM creation to minimize cost. This tier offers reliable, low-cost storage ideal for light workloads, testing environments, or non-critical applications._

![Disk Attachment - Diskt type - Select Standard HDD](screenshot/OS%20disk%20type%20Select%20Standard%20HDD%20VM%20Deployment.png)

### Step 23: Click Create and attach a new disk  
_Selected the option to create and attach a new data disk during VM setup to expand storage capacity for application files, logs, or persistent datasets beyond the OS volume._

![Disk Attachment - Attachment Button ](screenshot/Click%20Create%20and%20attach%20a%20new%20disk%20VM%20deployment%20.png)

### Step 24: Type DatBo1 and press Enter  
_Entered “DatBo1” as the disk name during creation to label and organize the new resource within the selected resource group. Naming conventions help ensure clarity across deployments and backups._

![Disk Attachment - Diskt Name](screenshot/Name-%20Rename%20the%20data%20disk%20VM%20deployment%20.png)

### Step 25: Click Change size  
_Opened the disk size selector during new disk creation to adjust capacity based on workload needs. Selected **32 GiB** for Premium SSD — suitable for fast boot volumes, app binaries, or small databases._

![Disk Attachment - Disk Size](screenshot/Size%20change%20Data%20Disk%20Size%20VM%20Deployment%20.png)

### Step 26: Click Storage type dropdown  
_Opened the storage type selector to compare disk tiers like Premium SSD, Standard SSD, and Ultra Disk. Each tier offers different IOPS, throughput, and burst capabilities tailored to workload performance needs._

![Disk Attachment - Disk Size](screenshot/Size%20Select%20storage%20type%20%20VM%20Deployment%20.png)

### Step 27: Select Standard HDD storage type  
_Selected “Standard HDD” from the storage type dropdown during disk creation to prioritize cost-efficiency. This tier offers reliable, low-throughput storage ideal for infrequent access workloads like backups, logs, or archival data._

![Disk Attachment - Storage Type](screenshot/Size%20change%20Storage%20type%20to%20Strandard%20HDD%20%20VM%20Deployment%20.png)

[Disk Attachment - Disk Size](screenshot/Size%20a%20disk%20size%2032GiB%20VM%20deployment%20.png)

[Disk Attachment - Disk Deletion Checkbox](screenshot/Delete%20click%20Delete%20disk%20with%20VM%20checkbox%20VM%20deployment.png)

[Disk Attachment - Compeletion](screenshot/Click%20OK%20new%20Disk%20tab%20VM%20deployment%20.png)

[Network Configuration - Network Tab](screenshot/Click%20Next%20Networking%20tab.png)

[Network Configuration - Virtual Network - Dropdown List ](screenshot/Virtual%20Network%20click%20dorpdown%20VM%20deployment.png)

[Network Configuration - Network vNeetprod](screenshot/Virtual%20Network%20select%20vNetprod%20VM%20deployment.png)

[Network Configuration - Subnet](screenshot/Subnet%20click%20dropdown%20VM%20deployment%20.png)

[Network Configuration - Subnet DEFUALT SUBNET](screenshot/Subnet%20select%20default%20subnet%20VM%20deployment%20.png)

[Network Configuration - Deletion IP & NIC Checkbox](screenshot/Delete%20click%20Delete%20public%20IP%20and%20NIC%20with%20VM%20checkbox%20VM%20deployment.png)

[Skipping Tabs - Management Tab as Defualt](screenshot/Click%20Next%20Management%20tab.png)

[Skipping Tabs - Monitoring Tab as Defualt](screenshot/Click%20Next%20Monitoring%20tab.png)

[Skipping Tabs - Advanced Tab as Defualt](screenshot/Click%20Next%20Advanced%20tab.png)

[Skipping Tabs - Tags Tab as Defualt](screenshot/Click%20Next%20Tags%20%20tab.png)

[Review Settings - Chekck Configured settings](screenshot/Review%20settings%20VM%20deployment%20.png)

[Deploy VM - Begin Deployment](screenshot/Click%20Create%20to%20begin%20Deployment%20%20VM%20deployment%20.png)

[Deployment Compeletion - GO TO Resources](screenshot/Click%20GO%20to%20Resources%20to%20view%20VM%20deployment.png)

## 📝 Reflection:


For over five hours, I wrestled with Git misfires, remote mismatches, authentication loops, and nested repo confusion—all while navigating the delicate structure of my Azure VM lab folder. Each error felt like a wall, but I treated every one as a lesson. I reconfigured remotes, corrected branch paths, and retraced my steps until the push finally landed. What began as a technical task became a test of patience and persistence. Now, my project lives on GitHub—not just as code, but as proof that I don’t quit when things get hard. I troubleshoot, I learn, and I finish strong.

