# 🖥️ Active Directory Forest Deployment & Domain Integration Lab

---

## 🧠 Objective

Deploy a new Active Directory forest using Windows Server 2016 and integrate multiple member servers into the domain.

---

## 🛠️ Technologies Used

- Windows Server 2016  
- Active Directory Domain Services (AD DS)  
- DNS  
- Server Manager  
- Hyper-V (Virtual Machines)  
- TCP/IP Configuration  
- Active Directory Users and Computers (ADUC)  

---

## 🏗️ Environment Overview

| Role | Server Name | Purpose |
|------|------------|----------|
| Domain Controller | RWDC31 | Forest Root Domain Controller |
| Member Server | Server31-A | Domain Member |
| Member Server | Server31-B | Domain Member |
| Storage Server | Storage31 | Domain Member |

**Forest Name:** `Domain31.local`

---

## ⚙️ Project Implementation

### 1️⃣ Installed Active Directory Domain Services

- Installed AD DS role using Server Manager  
- Promoted server to Domain Controller  
- Created a new forest (`DomainXX.local`)  
- Configured Directory Services Restore Mode (DSRM) password  
- Verified successful domain controller deployment  

---

### 2️⃣ Configured DNS for Domain Resolution

- Set Domain Controller IP as preferred DNS on member servers  
- Verified name resolution to domain controller  
- Confirmed domain authentication functionality  

---

### 3️⃣ Joined Servers to the Domain

- Joined:
  - Server31-A  
  - Server31-B  
  - Storage31  
- Authenticated using domain administrator credentials  
- Restarted systems to complete domain integration  
- Verified domain membership in Server Manager  

---

### 4️⃣ Validation & Verification

- Confirmed Domain Controller appears in **Domain Controllers OU**  
- Verified all member servers appear in **Computers container (ADUC)**  
- Successfully logged in using `domain31\Administrator`  
- Confirmed centralized authentication across all systems  

---

## 🔐 Skills Demonstrated

- Active Directory Forest Deployment  
- Domain Controller Promotion  
- DNS Configuration for AD Environments  
- Windows Server Administration  
- Enterprise Domain Integration  
- Active Directory Object Management  
- Troubleshooting Domain Join Issues  

---

## 📌 Key Takeaways

- Active Directory depends heavily on properly configured DNS  
- Domain join failures are often DNS-related  
- Centralized authentication simplifies enterprise administration  
- Proper validation ensures domain integrity and functionality  

---

## 📷 Screenshots

### Domain Controller OU
![Domain Controller OU](https://i.imgur.com/DMsaLhr.png)

---

### Server31-A – Local Server Page
![Server31-A](https://i.imgur.com/dTACmuf.png)

---

### Server31-B – Local Server Page
![Server31-B](https://i.imgur.com/AFg61rS.png)

---

### Storage31 – Local Server Page
![Storage31](https://i.imgur.com/S8yHoaO.png)

---

### ADUC Computers Container
![ADUC Computers Container](https://i.imgur.com/1NHf1Nf.png)

## 🚀 Project Outcome

Successfully deployed a fully functional Active Directory forest and integrated multiple member servers into the domain, simulating an enterprise-level Windows infrastructure environment.
