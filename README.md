# Setting Up an Active Directory Environment

**Introduction:** _The goal of this project is to learn how to install and configure Active Directory in a virtualized environment using tools like VMware or Hyper-V. By setting up a Domain Controller, configuring DNS, and understanding the role of Active Directory, this project will provide the foundational knowledge needed for managing users, groups, and resources in a networked environment._

Throughout this project, I'll gain hands-on experience with the following concepts and skills:

* Domain Setup: Learn how to create an Active Directory domain and understand its structure and components.
* Configuring DNS for AD: Understand the importance of DNS in an AD environment and set it up to ensure proper communication between servers and clients.
* Promoting a Server to Domain-Controller: Discover how to promote a server to a Domain Controller, which is responsible for managing authentication, user accounts, and network security within the domain.
* Understanding AD's Role in Networked Environments: Gain insight into how Active Directory is used to centralize identity management, control access to resources, and enforce security policies across a network.

**Tools:** To complete this project, I will use the following tools:

Windows Server: The operating system used to install and configure Active Directory.
Oracle VirtualBox: Virtualization software that allows you to create isolated virtual machines to simulate a real-world networked environment for Active Directory.

**Step 1: [Installation]**
Before diving into the good stuff it is important to install a virtual machine and Windows ISO image file.

**Install Oracle:**
https://www.virtualbox.org/

**Install Windows Server 2019 ISO image:**
https://www.microsoft.com/en-us/evalcenter/download-windows-server-2019

**Install Windows 10 ISO image:**
https://www.microsoft.com/en-us/software-download/windows10

_Based on your operating system, please verify and install the version of the software that matches your operating system architecture (either 64-bit or 32-bit). To determine which version you need, check whether your operating system is 64-bit or 32-bit._ You can view this by running **system-info** 
within the command prompt. 

**Step 2: [Installing Windows 2019 Server ISO] ** After the installation, you will open your Virtual Machine and import your ISO image by selecting **"NEW"**.
When creating a Virtual Machine for your Windows ISO image, please view the link below for support and visualization of my setup. https://drive.google.com/file/d/1DeyzcTVGCi0MqARtudVVC4cdmjc5-glg/view?usp=drive_link

**Step 3: [Changing Adapter Settings / Renaming PC]** After completing the installation, I configured the adapter settings for the Internal Network to connect to the DHCP server. Initially, the system was assigned an APIPA (Automatic Private IP Addressing) address in the 169.254.x.x range because it was unable to connect to the DHCP server. I then updated the adapter settings by statically configuring the IP address, subnet mask, and DNS server address. Following this configuration, I renamed the PC to "Domain Controller" to reflect its intended role within the network. Please view the link below.
https://drive.google.com/file/d/13jTdKZ3VL2RDE1bWniSmTqR2eD5s5O0d/view?usp=drive_link

Step 4: [Creating an OU Admin account / RAS/NAT installation]

