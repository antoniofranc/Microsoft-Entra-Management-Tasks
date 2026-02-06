# 🔐 Enable Azure Multi-Factor Authentication (MFA)

## 📘 Project Overview

Multi-Factor Authentication (MFA) is a foundational identity security control that requires users to verify their identity using **two or more authentication factors**, such as:
- Something you know (password)
- Something you have (mobile device, authentication app)
- Something you are (biometrics)

This project demonstrates how to **enable Azure MFA for a single user** in Microsoft Entra ID, following real-world IAM and security operations practices.

## 🎯 Learning Objectives

By completing this lab, I demonstrated the ability to:
- Enable Azure MFA for a specific user
- Understand MFA enforcement at the user level
- Configure authentication requirements in Microsoft Entra ID
- Apply identity security best practices to reduce account compromise
- Explain MFA implementation from an IAM and SOC perspective


## 🛠️ Technologies & Tools Used
- Microsoft Entra ID (Azure Active Directory)
- Azure Portal
- Azure MFA
- Authentication Methods
- User Management

📋 Step-by-Step Implementation
## 1️⃣ Access Microsoft Entra ID
- Logged into the Azure Portal
- Navigated to Microsoft Entra ID
- Selected Users
<img width="400" height="191" alt="image" src="https://github.com/user-attachments/assets/16857971-0467-4484-be06-a4718d24ba12" />
<img width="400" height="104" alt="image" src="https://github.com/user-attachments/assets/52ac249e-8f84-41ba-9083-64c9a5705fb3" />

## 2️⃣ Select Target User
- Chose a specific user account for MFA enforcement
- Verified user status and sign-in settings

<img width="400" height="322" alt="image" src="https://github.com/user-attachments/assets/fbfac7f0-320b-4e0e-9265-c5564bc270a9" />

## 3️⃣ Open Multi-Factor Authentication Settings
- Clicked Per-user MFA
- Opened the legacy MFA management portal
- Located the selected user

<img width="400" height="398" alt="image" src="https://github.com/user-attachments/assets/1b4ffa70-b445-48b7-8014-7c682360fea8" />

## 4️⃣ Enable MFA for the User
- Changed MFA status from:
- ❌ Disabled → ✅ Enabled
- Saved configuration
🔐 MFA is now enforced at sign-in for this user.

<img width="400" height="467" alt="image" src="https://github.com/user-attachments/assets/0c973517-a811-4314-b210-3907f607de3a" />
<img width="400" height="213" alt="image" src="https://github.com/user-attachments/assets/c07cfe29-54bd-42e8-83df-a0ddff9bf4db" />

## 5️⃣ Configure Authentication Methods
- Reviewed available MFA methods:
- Microsoft Authenticator app
- SMS verification
- Voice call (if enabled)
- Confirmed methods align with security policy

## 6️⃣ User MFA Registration Prompt
- On next sign-in, user is prompted to:
- Register MFA device
- Complete second-factor verification

<img width="400" height="176" alt="image" src="https://github.com/user-attachments/assets/0e1dd99b-c4cb-403e-95b3-8decb0ce51ac" />

## 7️⃣ Validate MFA Enforcement
- Confirmed MFA challenge occurs during login
- Access granted only after successful second-factor verification

<img width="400" height="289" alt="image" src="https://github.com/user-attachments/assets/91b0ec78-05de-4683-97c2-c424b03490ae" />
<img width="400" height="567" alt="image" src="https://github.com/user-attachments/assets/a55624ed-0a7c-4c62-843f-5adededc984a" />
<img width="418" height="323" alt="image" src="https://github.com/user-attachments/assets/925ee5ed-49d2-47be-a9a3-8da8f367cb1e" />
<img width="400" height="257" alt="image" src="https://github.com/user-attachments/assets/1de61e39-c072-4e00-bd61-27aa7bb4ea0b" />
<img width="400" height="291" alt="image" src="https://github.com/user-attachments/assets/bd3153c6-d430-48c8-b0e0-075bf42b6061" />
