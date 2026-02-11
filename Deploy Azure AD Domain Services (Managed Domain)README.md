# 🖥️ Deploy Azure AD Domain Services (Managed Domain)
## 📘 Project Overview

Azure Active Directory Domain Services (Azure AD DS) provides **managed domain** services such as:
- Domain join
- Group Policy
- Lightweight Directory Access Protocol (LDAP)
- Kerberos and NTLM authentication
- without requiring you to **deploy or manage domain controllers** in the cloud.

Azure AD DS integrates with your existing Azure AD tenant, letting users sign in with their existing credentials and use existing groups and user accounts to secure access. This enables a smooth **lift-and-shift of on-premises applications** to Azure.


📋 Step-by-Step Implementation

## 1️⃣ Access Azure AD Domain Services
- Logged into Azure Portal
- Navigated to Azure AD Domain Services
<img width="400" height="178" alt="image" src="https://github.com/user-attachments/assets/bce60176-c09f-4351-87a1-e18b97ba208c" />
<img width="400" height="231" alt="image" src="https://github.com/user-attachments/assets/8a159478-522d-4dee-9daa-018c4b934afc" />

## 2️⃣ Start Deployment
- Clicked Create Azure AD DS instance
- Entered DNS domain name
<img width="400" height="298" alt="image" src="https://github.com/user-attachments/assets/498da728-3851-4313-8ffc-b62a546690f9" />
<img width="400" height="293" alt="image" src="https://github.com/user-attachments/assets/3264bccc-ae42-41eb-8424-e8437a5e500d" />

## 3️⃣ Configure Resource Group & Region
- Selected existing resource group
- Chose Azure region for deployment
<img width="400" height="526" alt="image" src="https://github.com/user-attachments/assets/c7e827bf-3262-4391-a2f2-a5d92dda9f74" />
<img width="400" height="189" alt="image" src="https://github.com/user-attachments/assets/a7b4278d-915d-4c22-a9f8-2c284cecf165" />
<img width="400" height="88" alt="image" src="https://github.com/user-attachments/assets/8930ec94-969d-48fd-94b4-286886cbea47" />

## 4️⃣ Configure Network
- Selected Virtual Network
- Configured subnet for domain services
<img width="400" height="336" alt="image" src="https://github.com/user-attachments/assets/4c7cbd20-913e-465b-8131-547969b76dbf" />
<img width="400" height="442" alt="image" src="https://github.com/user-attachments/assets/23b0f6f8-5641-495a-84d4-d1c7ddaeb773" />

## 5️⃣ Select Azure AD Domain Service Administrators 
- Manage Group Membership 
- Chose admin Account 
<img width="400" height="373" alt="image" src="https://github.com/user-attachments/assets/92c8abc6-9252-4e2a-bf1d-22f4e9a70f3a" />
<img width="400" height="240" alt="image" src="https://github.com/user-attachments/assets/01596e88-96fc-451b-b8a6-155570315d7c" />
<img width="400" height="399" alt="image" src="https://github.com/user-attachments/assets/6362afa1-cfae-49fa-83e7-9da1cebace97" />

## 6️⃣ Review & Create
- Return to set up 
- Clicked Create to provision Azure AD DS
- Sync all users
- Review youer Settings
<img width="400" height="204" alt="image" src="https://github.com/user-attachments/assets/1c50a02c-9d2e-4782-b209-4f4751459e87" />
<img width="400" height="765" alt="image" src="https://github.com/user-attachments/assets/cf767cde-4971-4df3-bb3f-213c56abcbdc" />
<img width="400" height="361" alt="image" src="https://github.com/user-attachments/assets/a06a2013-c4f2-4b91-979f-274626f31e53" />
<img width="400" height="191" alt="image" src="https://github.com/user-attachments/assets/ea04059f-a44c-4f32-bb4c-c62671e3b060" />
<img width="400" height="410" alt="image" src="https://github.com/user-attachments/assets/e342708b-faba-404f-a6f2-22f4e4250279" />

## 7️⃣ Verify Domain Deployment
- Deployment completed successfully
- Verified DNS domain, OU structure, and synchronized users
- View the health of the deployment
- Click the warning
- Fix  DNS
<img width="400" height="277" alt="image" src="https://github.com/user-attachments/assets/3afd4846-0c7d-46ae-9721-4e5b25a3878d" />
<img width="400" height="404" alt="image" src="https://github.com/user-attachments/assets/f1ee02f7-5c5e-4e03-9c62-fcdeeb2243ab" />
<img width="400" height="546" alt="image" src="https://github.com/user-attachments/assets/3146f575-d2b1-4672-b76f-1b0328e9fc7e" />
<img width="400" height="435" alt="image" src="https://github.com/user-attachments/assets/73d9045a-1a0a-4b8c-8e65-e7c4e731a630" />
<img width="400" height="249" alt="image" src="https://github.com/user-attachments/assets/ef8a873b-dac7-44b7-ac5a-15c6ca909b4e" />
<img width="400" height="279" alt="image" src="https://github.com/user-attachments/assets/1dc17c5f-e19a-4113-8446-72168b9b1a81" />
<img width="400" height="188" alt="image" src="https://github.com/user-attachments/assets/700ae192-5347-4cd8-a1bd-c43ec5908145" />
<img width="400" height="386" alt="image" src="https://github.com/user-attachments/assets/5767470e-1772-4038-a506-488994b1432b" />
<img width="400" height="428" alt="image" src="https://github.com/user-attachments/assets/1e213ad5-64a7-40d8-a1e7-eb33a8e5d7ea" />
<img width="400" height="313" alt="image" src="https://github.com/user-attachments/assets/7dc69cda-1ad6-4315-a026-a4ffa2f2bb90" />
<img width="400" height="172" alt="image" src="https://github.com/user-attachments/assets/33ba07d0-6346-45f7-9a2b-57d480143afb" />
<img width="401" height="142" alt="image" src="https://github.com/user-attachments/assets/2321c1fd-8a94-4d95-9bd6-fdcd82603ceb" />

## 8️⃣ Check DNS Setting 
- Virtual Network
- Check the IP address is selected 
<img width="690" height="410" alt="image" src="https://github.com/user-attachments/assets/884b02f5-9c54-4af8-b336-ee15327eb46b" />
<img width="619" height="595" alt="image" src="https://github.com/user-attachments/assets/f558560a-450e-4eb0-9b08-f44ce28fdbd9" />
<img width="379" height="589" alt="image" src="https://github.com/user-attachments/assets/dd3b6feb-1aa8-4fa8-b312-990799cd0ea5" />
<img width="350" height="154" alt="image" src="https://github.com/user-attachments/assets/a2238f07-1ad0-4051-ac60-47587dc6f28f" />

