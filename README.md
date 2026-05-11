# windows-server-file-sharing-access-control
Windows Server file sharing project using shared folders, NTFS permissions, security groups, mapped drives, and basic access control.

# Windows Server File Sharing and Access Control

## Overview

I created this project to better understand how file sharing works in a Windows Server environment. The goal was to practice setting up shared folders, managing permissions, and testing user access like it would be done in a business environment.

This helped me understand how companies control access to shared files instead of storing everything locally on individual computers.

---

## What I Built

In this setup, I configured:

- Shared folders on Windows Server
- Folder permissions using the Security tab
- Share permissions
- Domain user access
- Security groups
- Mapped network drives
- Basic Group Policy testing

---


| Component | Details |
|---|---|
| Server | Windows Server 2022 |
| Client | Windows 11 Pro |
| Domain | Active Directory Domain |
| Tools Used | Server Manager, File Explorer, Active Directory Users and Computers, Group Policy Management |

---

## Shared Folder Setup

I created a shared folder on the server so it could be accessed from another computer on the network.

The purpose of this was to understand how shared drives work in companies, where files are stored on a server and users access them based on permissions.

---

## Permissions and Security

I worked with both sharing permissions and security permissions.

The main thing I learned is:

```text
Sharing permissions = can the user reach the folder over the network?
Security permissions = what can the user actually do inside the folder?
```

For example, a user may be able to open a folder but not edit or delete files depending on the permissions assigned.

---

## Security Groups

Instead of giving permissions to individual users one by one, I practiced using groups.

This is important because in real environments, administrators usually assign permissions to groups instead of separate users.

Example:

```text
HR Users → access to HR folder
IT Users → access to IT folder
Regular Users → limited access
```

This makes access easier to manage as users are added or removed.

---

## Mapped Drive Testing

I also tested mapping a shared folder as a network drive.

This allows users to access a shared folder more easily from File Explorer instead of typing the full network path every time.

Example:

```text
\\ServerName\ShareName
```

Mapped drives are commonly used in workplaces so employees can quickly access shared resources.

---

## Group Policy Testing

I practiced basic Group Policy configuration to see how settings can be pushed to users or computers in a domain environment.

This helped me understand how administrators can manage multiple computers from one central location instead of configuring each machine manually.

---

## What I Tested

I tested:

- Accessing the shared folder from another machine
- Logging in as a domain user
- Checking if permissions applied correctly
- Verifying whether users could read, edit, or access files
- Mapping a shared folder as a drive
- Applying basic policy settings

---

## What I Learned

This project helped me understand:

- How shared folders work in Windows Server
- The difference between share permissions and NTFS/security permissions
- Why groups are better than assigning permissions to individual users
- How mapped drives help users access shared folders
- How file access is controlled in a domain environment
- How permissions connect to real IT support issues

---

## Real-World Connection

This is useful because file sharing and permissions are common in IT jobs.

Examples of real issues this connects to:

- A user cannot access a shared drive
- A user has read-only access but needs edit permissions
- A department needs a private folder
- A mapped drive is not showing
- A user is in the wrong security group

This project helped me understand how to troubleshoot those types of problems.

---

## Screenshots

### Shared Folder Created on Server
Created a shared folder on the Windows Server machine so it could be accessed from another computer on the network.

<img width="1133" height="677" alt="Screenshot 2026-05-10 195647" src="https://github.com/user-attachments/assets/61c8e3ae-f728-41c7-8c4b-9f8598663090" />

---

### Security Permissions
Configured folder security permissions to control what users are allowed to do inside the folder, such as read, write, modify, or delete files.

<img width="427" height="541" alt="Screenshot 2026-05-11 131917" src="https://github.com/user-attachments/assets/2af9c894-b710-452d-a6c0-58520b384620" />

---

### Share Permissions
Reviewed share permissions to understand how network access works together with NTFS/security permissions.

<img width="605" height="443" alt="Screenshot 2026-05-11 132202" src="https://github.com/user-attachments/assets/3da1963e-24c8-445b-ab2f-abf68713702a" />

---

### Security Group Configuration
Created and used security groups to manage folder access instead of assigning permissions to each user individually.

<img width="428" height="466" alt="Screenshot 2026-05-11 132352" src="https://github.com/user-attachments/assets/e3c919b0-a131-42e3-a0dc-5fd93277deba" />

---

### Mapped Drive Access
Mapped the shared folder as a network drive so the user could access it easily from File Explorer.

<img width="555" height="417" alt="Screenshot 2026-05-10 212420" src="https://github.com/user-attachments/assets/cd4f0a14-e0b8-445f-af84-6fe481f59317" />

---

### Group Policy Testing
Tested basic Group Policy settings to understand how administrators can apply settings to domain users or computers from one place. (wallpapers)

<img width="686" height="625" alt="Screenshot 2026-05-11 123700" src="https://github.com/user-attachments/assets/8c8d3aa1-24b6-4db7-a30f-9180e34e5eaa" />


### Additoinal Notes under /notes
for details.
