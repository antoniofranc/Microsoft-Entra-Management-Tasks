# 🔐 Azure Entra ID – Configure and Enable User Risk Policy

## 📌 Project Overview
This hands-on lab demonstrates how to configure and enable a **User Risk Policy** using Microsoft Entra ID (formerly Azure AD) Identity Protection.

Identity Protection evaluates user behavior and calculates risk signals to determine the probability that an identity has been compromised. Based on this risk score, administrators can enforce automated remediation policies such as:
- Block access
- Allow access
- Require password reset (Self-Service Password Reset)

This lab focuses on enabling a **User Risk Policy** that forces high-risk users to reset their password.

---
## 🎯 Learning Objectives

- Understand Microsoft Entra ID Identity Protection
- Configure User Risk Policy
- Enforce password reset for high-risk users
- Enable self-service remediation
- Understand automated risk-based access control

---
### Step 1 – Navigate to Identity Protection
1. Login to Azure Portal
2. Go to **Microsoft Entra ID**
3. Select **Protection → Identity Protection**

<img width="300" height="183" alt="image" src="https://github.com/user-attachments/assets/376fde5e-9e1b-418a-875f-e4817e07ad73" />
<img width="300" height="165" alt="image" src="https://github.com/user-attachments/assets/0192604d-41e9-4e54-8737-a6e9ab44b157" />
<img width="300" height="334" alt="image" src="https://github.com/user-attachments/assets/963a02b3-14bc-4ee5-b0d7-35b24b723518" />

---

### Step 2 – Review Risk Overview

- View User Risk Levels
- View Sign-in Risk Levels
- Analyze detected risk events

<img width="400" height="351" alt="image" src="https://github.com/user-attachments/assets/279b4bbf-1b24-4c23-8f61-5f318b292d26" />
<img width="400" height="326" alt="image" src="https://github.com/user-attachments/assets/fb4a436a-1ec5-4e1d-92de-6dc3f584449d" />


### Step 3 – Configure User Risk Policy

1. Navigate to:
   Identity Protection → User Risk Policy

2. Configure:
   - Assignments → Include All Users
   - Conditions → User risk level: High
   - Access → Require password change

3. Enable Policy → ON

<img width="400" height="291" alt="image" src="https://github.com/user-attachments/assets/2e983b53-fc8a-4662-87d3-089c45bc6cdc" />
<img width="400" height="396" alt="image" src="https://github.com/user-attachments/assets/e2e0926c-ef21-4ab0-b39b-24251a99bb11" />

----

### Step 4 – Enable Self-Service Password Reset (SSPR)

1. Go to:
   Entra ID → Password Reset

2. Enable:
   - Self-Service Password Reset for All Users

3. Configure authentication methods

<img width="400" height="226" alt="image" src="https://github.com/user-attachments/assets/c0b88b24-932f-4e35-b115-7e66e35d8be7" />
<img width="400" height="175" alt="image" src="https://github.com/user-attachments/assets/b9b7e790-1628-4064-9d52-1869cc79037d" />
<img width="400" height="495" alt="image" src="https://github.com/user-attachments/assets/b98ee23b-2654-43f6-befa-3acd9e00df84" />



<img width="400" height="256" alt="image" src="https://github.com/user-attachments/assets/94dcaddc-2136-4eb6-abb3-2a4ea27bc1d3" />
<img width="400" height="160" alt="image" src="https://github.com/user-attachments/assets/17420234-5ec2-4dbb-beb0-1bc7b622972d" />
<img width="400" height="234" alt="image" src="https://github.com/user-attachments/assets/2dc8730f-da8c-460d-b687-90aec4e4f88e" />
<img width="400" height="183" alt="image" src="https://github.com/user-attachments/assets/f803b85e-96db-462f-93e5-59fbd623efd1" />
<img width="400" height="249" alt="image" src="https://github.com/user-attachments/assets/dc409cba-7552-425e-a0b7-ae970f5271c5" />

-----

## 🔐 Security Impact

When a user is flagged as **High Risk**, the system:

- Blocks access until password reset
- Allows self-remediation
- Automatically closes the risk event
- Reduces administrative overhead

---

Organizations use Identity Protection to:

- Prevent account takeover attacks
- Mitigate credential stuffing
- Reduce insider threat risks
- Enforce adaptive security controls

---
