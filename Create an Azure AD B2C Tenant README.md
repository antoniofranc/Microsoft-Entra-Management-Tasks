# 🧾 Create an Azure AD B2C Tenant (Customer Identity Management)
## 📘 Project Overview

Azure Active Directory B2C (Azure AD B2C) is Microsoft’s **Customer Identity and Access Management (CIAM)** platform. It allows organizations to manage **customer identities** for applications and APIs, enabling sign-in with:
- Social identities (Google, Facebook, etc.)
- Local accounts (email & password)
- Enterprise identities

An **Azure AD B2C tenant is separate and distinct** from a standard Azure AD (Microsoft Entra ID) tenant and is purpose-built for **external customer** authentication, not internal employees.

## 🎯 Learning Objectives
By completing this lab, I demonstrated how to:
- Understand the difference between Azure AD and Azure AD B2C
- Create a new Azure AD B2C tenant
- Configure tenant basics (name, domain, region)
- Link the B2C tenant to an Azure subscription
- Prepare the environment for customer authentication scenarios

📋 Step-by-Step Implementation
## 1️⃣ Access the Azure Portal
- Click the hamburger
- Click all service 

<img width="400" height="120" alt="Screenshot 2026-02-09 010536" src="https://github.com/user-attachments/assets/107e0c14-1fce-4d79-9f2c-5c1bcaaa10c2" />
<img width="400" height="226" alt="Screenshot 2026-02-09 010554" src="https://github.com/user-attachments/assets/f99c47a9-da8b-4757-81c3-bfb3d1811527" />

## 2️⃣ Access Subscriptions 
- Click subscriptions
- Resource providers
- Confirm Microsoft.AzureActiveDirectory is registered 
<img width="400" height="318" alt="Screenshot 2026-02-09 010608" src="https://github.com/user-attachments/assets/ce9474aa-b3df-421d-8134-bae8176e0f66" />
<img width="400" height="421" alt="Screenshot 2026-02-09 010633" src="https://github.com/user-attachments/assets/0e44efba-ece7-4374-a2d0-87981c046978" />
<img width="400" height="728" alt="Screenshot 2026-02-09 010919" src="https://github.com/user-attachments/assets/38e637c6-0af2-4f38-b9fd-ff584254d256" />
<img width="400" height="546" alt="Screenshot 2026-02-09 010943" src="https://github.com/user-attachments/assets/23f681b3-cc49-4e71-8baf-8d46a565af5e" />

## 3️⃣ Create Resource
- Create resources
- Select Azure Active Directory B2C
<img width="400" height="267" alt="Screenshot 2026-02-09 011012" src="https://github.com/user-attachments/assets/b64b484d-bd9c-4c1c-86ec-326fe2a8dca4" />
<img width="400" height="305" alt="Screenshot 2026-02-09 011208" src="https://github.com/user-attachments/assets/8f1f50fa-694c-483e-9f43-981730dca645" />
<img width="400" height="768" alt="Screenshot 2026-02-09 011248" src="https://github.com/user-attachments/assets/0d95c2ec-1fdd-4978-a2e8-a4c60d68acb0" />
<img width="400" height="529" alt="Screenshot 2026-02-09 011303" src="https://github.com/user-attachments/assets/0e527dd6-e79e-4c46-8bb2-aee384ed9908" />

## 4️⃣ Start B2C Tenant Creation
- Select create a new Azure AD B2C Tenant
- Create a Tenant
- click the success message 
<img width="400" height="353" alt="Screenshot 2026-02-09 011318" src="https://github.com/user-attachments/assets/5a39d0b3-ec20-4021-828a-4ebcc696a15f" />
<img width="400" height="761" alt="Screenshot 2026-02-09 011441" src="https://github.com/user-attachments/assets/84f2e487-3446-4bff-8502-ec8cfd1f04c7" />
<img width="400" height="761" alt="Screenshot 2026-02-09 011459" src="https://github.com/user-attachments/assets/9ecbaf1d-e41d-4f52-9adb-b4f6cb78878d" />
<img width="400" height="582" alt="Screenshot 2026-02-09 011511" src="https://github.com/user-attachments/assets/06fea220-86ce-4b77-b7ad-d2091e3396b3" />
