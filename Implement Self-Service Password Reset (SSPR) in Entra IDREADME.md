# 🔐 Enable Self-Service Password Reset (SSPR) in Microsoft Entra ID

## Lab Overview
Azure Active Directory self-service password reset (SSPR) gives users the ability to change or reset their password, with no administrator or help desk involvement. If a user’s account is locked or they forget their password, they can follow prompts to unblock themselves and get back to work. This ability reduces help desk calls and loss of productivity when a user can’t sign in to their device or an application.

This capability:
- Reduces help desk tickets
- Improves user productivity
- Strengthens identity security through verification methods


## 📋 Step-by-Step Implementation

## 1️⃣ Access Microsoft Entra ID
- Logged into the Azure Portal
- Navigated to Microsoft Entra ID
- Selected Password reset
<img width="400" height="628" alt="image" src="https://github.com/user-attachments/assets/ccd251fc-564f-4f76-86da-3cb658159c72" />

## 2️⃣ Enable SSPR for a Selected Group
- Set Self-service password reset enabled to:
- ✅ Selected
- Chose a security group instead of “All users”
🔐 This follows least privilege and phased deployment best practices.

<img width="400" height="355" alt="image" src="https://github.com/user-attachments/assets/7a925c3e-dab0-49ca-8a8b-59bcdf42f61d" />

<img width="400" height="445" alt="image" src="https://github.com/user-attachments/assets/8e986419-f3fe-458f-b4ba-acef820fd040" />
<img width="400" height="349" alt="image" src="https://github.com/user-attachments/assets/080d84e0-dc8f-4577-8b0e-fa5b2e4bbaa4" />
<img width="400" height="228" alt="image" src="https://github.com/user-attachments/assets/fa8e4287-0ebb-49d0-865d-7de3151ea741" />

## 3️⃣ Configure Authentication Methods
- Navigated to Authentication methods
- Selected the allowed verification methods:
- Mobile app notification
- Mobile app code
- Email
- Security questions (optional based on org policy)

<img width="400" height="450" alt="image" src="https://github.com/user-attachments/assets/27e4b84b-1084-41f0-9544-2495f43ce503" />


<img width="530" height="361" alt="image" src="https://github.com/user-attachments/assets/8ea7b1e8-d186-4c96-978c-aeb109d5411c" />


## 4️⃣ Define Reset Requirements
- Configured:
- Number of authentication methods required
- Methods available for password reset vs. password change
- Ensured security requirements meet enterprise standards

<img width="768" height="334" alt="image" src="https://github.com/user-attachments/assets/bb5498d8-7135-4ae6-965c-43ab79168d82" />

## 5️⃣ Review Registration Settings

- Confirmed users are prompted to register authentication info
- Ensured registration is required before using SSPR


## 6️⃣ Validate Configuration
- Confirmed:
- SSPR is enabled
- Group targeting is correct
- Authentication methods are active
- Configuration is now ready for end users














