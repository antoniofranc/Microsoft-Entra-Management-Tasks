# Add a Custom Domain Name to Azure AD

## Lab Overview
Every new Azure AD tenant comes with an initial domain name in the format `domainname.onmicrosoft.com`. While you cannot change or delete this initial domain name, you can add custom domain names that are familiar to your users and organization.

This lab walks you through the complete process of:
- Adding a custom domain to Azure AD
- Creating DNS TXT records for domain verification
- Verifying domain ownership
- Setting the custom domain as primary

## Learning Objectives
The process of adding a new custom domain to a new Azure AD tenant. You’ll add the domain, create the necessary TXT records to verify the domain , and then you will verify the domain. You’ll wrap up by making the custom domain primary.


## 📋 Step-by-Step Implementation
1️⃣ Access Microsoft Entra ID
- Logged into the Azure Portal
- Navigated to Microsoft Entra ID
- Selected Custom domain names
<img width="400" height="245" alt="image" src="https://github.com/user-attachments/assets/a2729dde-5a2d-4703-b04c-ad55339198dc" />

<img width="400" height="718" alt="image" src="https://github.com/user-attachments/assets/2ec3174c-3a04-4d88-a74f-396c0ecede9e" />

## 2️⃣ Add a Custom Domain
- Clicked Add custom domain
- Entered the domain name (example: exampledomain.com)
- Initiated domain verification

<img width="500" height="284" alt="image" src="https://github.com/user-attachments/assets/658bf739-472e-4a60-a35a-858b4decfc92" />
<img width="500" height="155" alt="image" src="https://github.com/user-attachments/assets/36463fe4-c0da-4480-9536-470d3b112c38" />

## 3️⃣ Retrieve DNS Verification Record
- Microsoft Entra ID generated a TXT record
- TXT record includes:
- Host/Name
- Value
- TTL

<img width="400" height="486" alt="image" src="https://github.com/user-attachments/assets/5aab7d0f-d4fd-4e5a-b410-f15b97d7838e" />


## 4️⃣ Create TXT Record in DNS Provider
- Logged into domain DNS provider
- Created the TXT record exactly as provided by Entra ID
- Saved DNS configuration

<img width="500" height="575" alt="image" src="https://github.com/user-attachments/assets/cb0a2d03-745a-4ec9-9039-642cd0c5698d" />

## 5️⃣ Verify Domain Ownership
- Returned to Microsoft Entra ID
- Clicked Verify
- Domain verification succeeded after DNS propagation

<img width="500" height="733" alt="image" src="https://github.com/user-attachments/assets/d85d6753-1fa0-445e-aeb0-65c8bb9ab21e" />

## 6️⃣ Set Custom Domain as Primary
- Selected the verified domain
- Set it as the Primary Domain
- Confirmed that future users will use this domain by default

<img width="500" height="297" alt="image" src="https://github.com/user-attachments/assets/8edeb39f-d378-44fb-a7af-3cce5f8a39a2" />




