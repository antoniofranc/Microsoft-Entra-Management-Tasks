# 🔐 Azure Entra ID – Assign Azure AD Role Using PIM

## 📌 Project Overview

This hands-on lab demonstrates how to assign the **Application Administrator** role using Microsoft Entra Privileged Identity Management (PIM).

Privileged Identity Management (PIM) enables Just-In-Time (JIT) privileged access to Azure AD roles, reducing standing administrative privileges and enforcing security controls such as:

- Time-based access
- Approval-based activation
- MFA enforcement
- Audit logging
- Access reviews

This lab focuses on assigning a user as **Eligible** for the Application Administrator role and activating the role through PIM.

----
## 🔎 Lab Walkthrough

### Step 1 – Navigate to PIM

1. Login to Azure Portal
2. Go to **Microsoft Entra ID**
3. Select:
   Identity Governance → Privileged Identity Management
<img width="400" height="278" alt="image" src="https://github.com/user-attachments/assets/8a20efdb-9457-4b81-aca3-747eb97924a8" />
<img width="400" height="434" alt="image" src="https://github.com/user-attachments/assets/6a067862-cbd6-49b7-ab0d-880f58059ab8" />

---

### Step 2 – Manage Azure AD Roles

1. Select **Azure AD Roles**
2. Choose **Roles**
3. Locate:
   Application Administrator

<img width="284" height="468" alt="image" src="https://github.com/user-attachments/assets/9e4a4145-2a2d-44d3-bb6f-e8c5e8ff1630" />
<img width="300" height="273" alt="image" src="https://github.com/user-attachments/assets/2bce5100-ed6c-4c82-8c5e-77868a8d0334" />
<img width="300" height="467" alt="image" src="https://github.com/user-attachments/assets/e3cce6b8-485a-4915-bf2c-14ebb6b95c98" />

---
### Step 3 – Add Role Assignment

1. Click **Add Assignments**
2. Select:
   - Member Type → Eligible
   - Select User
3. Configure:
   - Assignment duration
   - Justification requirement

Save configuration.

<img width="300" height="593" alt="image" src="https://github.com/user-attachments/assets/cdd87a6d-5bf3-4cb3-b86a-b6d567c126e5" />
<img width="300" height="446" alt="image" src="https://github.com/user-attachments/assets/5d2dcfed-3ae9-47df-a947-b397cbd2340c" />
<img width="300" height="764" alt="image" src="https://github.com/user-attachments/assets/42347969-51a3-43ea-959b-b9470452ea83" />
<img width="300" height="383" alt="image" src="https://github.com/user-attachments/assets/b3729fb3-e3ce-442f-abb8-0fa43e39022a" />
<img width="300" height="772" alt="image" src="https://github.com/user-attachments/assets/bbbb6d1e-a21c-45d0-9274-02769f308fdc" />

---
### Step 4 – Configure Role Settings

Configure activation requirements:

- Require MFA
- Require justification
- Set maximum activation duration
- Require approval (optional)

---
### Step 5 – Activate the Role

User performs:

1. Go to:
   PIM → My Roles
2. Select:
   Application Administrator
3. Click **Activate**
4. Provide justification
5. Complete MFA challenge

Role becomes active for defined time period.

<img width="400" height="499" alt="image" src="https://github.com/user-attachments/assets/3986825e-1876-4ecb-930d-d75b373215f4" />
<img width="400" height="317" alt="image" src="https://github.com/user-attachments/assets/bf8f0112-7bde-42f8-a49d-e0fa4ebcc1d9" />


### Step 6 – Review Audit Logs

Navigate to:

Entra ID → Audit Logs

Verify:

- Role assignment
- Activation event
- Approval workflow (if enabled)

---

## 🔐 Security Impact

Without PIM:
- Admin roles are permanently assigned (standing privilege)

With PIM:
- Access is temporary
- Requires approval
- Enforces MFA
- Fully logged
- Reduces attack surface

---





















