# 💻 Azure Entra ID – Configure Device Join Permissions

## 📌 Project Overview

This hands-on lab demonstrates how to configure device settings in Microsoft Entra ID (Azure AD), specifically allowing a **specific user** to join devices to Azure Active Directory.

Microsoft Entra ID provides centralized identity management for:

- Users
- Groups
- Devices
- Applications

Controlling which users can join devices to Azure AD is critical for maintaining secure device enrollment and enforcing Zero Trust security principles.


## 🔎 Lab Walkthrough

### Step 1 – Navigate to Devices

1. Login to Azure Portal
2. Go to:
   Microsoft Entra ID
3. Select:
   Devices

<img width="300" height="605" alt="image" src="https://github.com/user-attachments/assets/7c3edde9-2703-4794-b3f7-099944b20187" />


---

### Step 2 – Open Device Settings

1. Click:
   Device Settings

2. Locate:
   "Users may join devices to Azure AD"

<img width="400" height="357" alt="image" src="https://github.com/user-attachments/assets/e47f2927-95f1-4a73-a195-30bfd34c3de3" />

---

### Step 3 – Configure Join Permissions

Change setting from:

- All → Selected

Then:

- Select specific user
- Save configuration

This ensures only approved identities can register devices.


<img width="300" height="300" alt="image" src="https://github.com/user-attachments/assets/da38dae3-06a5-4cbe-9708-b1c3d6d7b4f4" />
<img width="300" height="330" alt="image" src="https://github.com/user-attachments/assets/25b056c9-2f7f-4531-8065-750cf98b2828" />
<img width="300" height="289" alt="image" src="https://github.com/user-attachments/assets/07e6f80c-2467-45ae-9878-fd64cc0ce97a" />
<img width="300" height="734" alt="image" src="https://github.com/user-attachments/assets/457e243c-14a5-464d-adc7-168695457fff" />
<img width="300" height="767" alt="image" src="https://github.com/user-attachments/assets/060d1dd9-a40c-4394-8b44-1794a251d026" />

----
### Step 4 – Verify Device Registration

After configuration:

- User joins device to Azure AD
- Device appears under:
  Entra ID → Devices → All Devices

Verify:

- Join type
- Owner
- Compliance status


<img width="400" height="487" alt="image" src="https://github.com/user-attachments/assets/96f4804a-5244-4c1f-aca3-d47f70d1a929" />
<img width="400" height="460" alt="image" src="https://github.com/user-attachments/assets/ae8df6d8-120e-4ee0-a055-e6c410651572" />

### Step 5 – Review Audit Logs

Navigate to:

Entra ID → Audit Logs

Confirm:

- Device join setting change
- Device registration activity

---

## 🔐 Security Impact

If "All Users" can join devices:

- Increased attack surface
- Unauthorized device registrations
- Potential lateral movement

By restricting to specific users:

- Enforced device governance
- Reduced shadow IT risk
- Improved endpoint visibility
- Stronger Zero Trust posture
