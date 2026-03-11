# active-directory-iam-home-lab
Hands-on Identity and Access Managment home lab using VirtualBox, Windows Server 2022, and Active Directory

## Active Directory IAM Home Lab – Windows Server 2022

### Overview

This project demonstrates a basic **Identity and Access Management (IAM) environment** built using **Windows Server 2022 and Active Directory** inside a VirtualBox virtual machine.

The goal of this lab was to simulate how organizations manage **user identities, authentication, and role-based access control (RBAC)** within an enterprise network.

This project is part of my cybersecurity training while preparing for **CompTIA Security+ and IAM-focused roles**.

---

# Lab Environment

Host Machine
Windows 11

Virtualization Platform
Oracle VirtualBox

Server Operating System
Windows Server 2022 Evaluation

Domain Name
corp.local

Server Role
Domain Controller

---

# Step 1 – Install VirtualBox

VirtualBox was installed on the Windows 11 host machine to create a virtualized lab environment.

Virtual machines allow cybersecurity professionals to simulate enterprise networks without affecting the host system.

---

# Step 2 – Install Windows Server 2022

A new virtual machine was created with:

Memory: 4096 MB
CPU: 2 Processor
Disk: 50 GB

Windows Server 2022 was installed using the Microsoft evaluation ISO.

The **Desktop Experience version** was selected to allow GUI-based administration tools.

---

# Step 3 – Promote Server to Domain Controller

The **Active Directory Domain Services (AD DS)** role was installed using Server Manager.

The server was then promoted to a **Domain Controller**, creating a new Active Directory forest:

Domain Name:
corp.local

The Domain Controller is responsible for:

* User authentication
* Identity management
* Security policy enforcement
* Access control across the network

---

# Step 4 – Active Directory Setup

The following management tool was used:

Active Directory Users and Computers

This console allows administrators to manage:

* Users
* Groups
* Organizational Units
* Access permissions

---

# Step 5 – Identity Object Creation

User accounts were created to simulate employees within an organization.

Example user created:

Sarah Jones
Username: sjones
Location: corp.local/Users

This simulates a real employee identity inside the company directory.

---

# Step 6 – Role-Based Access Control (RBAC)

Security groups were created to simulate **department-based access control**.

Groups created:

Finance
HR

These groups represent organizational roles.

Users are assigned to groups rather than granting permissions directly to users.

Example:

Sarah Jones → Member of Finance Group

This demonstrates **RBAC (Role-Based Access Control)**, a core Identity and Access Management principle used in enterprise environments.

---

# IAM Concepts Demonstrated

Identity Lifecycle Management
User Account Provisioning
Active Directory Domain Services
Role-Based Access Control (RBAC)
Centralized Authentication
Domain Controller Architecture

---

# Screenshots

(Screenshots of the following were captured)

* Active Directory Users and Computers
* User creation (Sarah Jones)
* Finance group membership
* HR security group
<img width="998" height="844" alt="Screenshot 2026-03-09 165615" src="https://github.com/user-attachments/assets/d18cab13-b45b-4d7c-9679-af09c653bd46" />
<img width="991" height="785" alt="Screenshot 2026-03-09 193106" src="https://github.com/user-attachments/assets/a5726eef-c7ec-4d46-bd87-b6b6edca8d90" />
<img width="987" height="785" alt="Screenshot 2026-03-09 193327" src="https://github.com/user-attachments/assets/afb822a4-f3ed-4a3f-9eca-34c3a7f21499" />


---

# Future Enhancements

This lab will continue with:

Group Policy (GPO)
Password policies
Account lockout configuration
Helpdesk password reset delegation
Domain-joined workstation testing

---

# Skills Demonstrated

Active Directory Administration
Identity and Access Management
Windows Server Administration
RBAC Implementation
Enterprise Directory Services

---

# Why This Matters

Organizations rely on Active Directory and IAM frameworks to manage user identities and control access to sensitive systems.

This lab demonstrates hands-on experience with **core identity management tasks performed by IT and cybersecurity professionals**.

---

# The Trick For GitHub (Quick Tip)

When you upload your screenshots:

Name them like this:

```
create_user.png
finance_group.png
hr_group.png
active_directory_console.png
```

Then reference them like this:

```
![User Creation](images/create_user.png)
```

GitHub will show them automatically.

---

# What You Have Actually Built (This Is Big)

You now have experience with:

* Domain Controllers
* Active Directory
* Identity creation
* RBAC
* Group membership management

These appear in **IAM analyst job descriptions constantly**.



---

If you want, I can also show you **one small trick that makes this lab look 10x more impressive on a resume** and helps IAM recruiters notice you faster.
