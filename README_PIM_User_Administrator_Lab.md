# 🔐 HANDS-ON AZURE LAB  
## Privileged Identity Management (PIM) – Assign & Activate User Administrator Role

---

## 📌 Lab Overview
In this lab, I configured **Microsoft Entra Privileged Identity Management (PIM)** to enforce **Just-In-Time (JIT) access control**.


- Assigned **Adam Young** as **Eligible** for the **User Administrator role**
- Configured **MFA using Microsoft Authenticator**
- Logged in as Adam and **activated the role securely**

This simulates a **real-world IAM workflow** used in enterprise environments.

---

## 🎯 Learning Objectives
- Implement **Privileged Identity Management (PIM)**
- Assign **Eligible (temporary) admin access**
- Enforce **Multi-Factor Authentication (MFA)**
- Activate roles using **Just-In-Time (JIT) access**
- Understand **least privilege security model**

---

## 🧱 Architecture
| Component | Purpose |
|----------|--------|
| Microsoft Entra ID | Identity provider |
| PIM | Controls privileged access |
| User Administrator | Role for managing users |
| MFA | Adds security verification |
| Eligible Assignment | Temporary role access |

---

# 🛠️ Step-by-Step Implementation

---

## 🔹 Step 1 – Sign in to Azure
Log in to the Azure portal.



---

## 🔹 Step 2 – Go to All Services
Click **All Services**.



---

## 🔹 Step 3 – Search for Entra Services
Search for **Entra**.



---

## 🔹 Step 4 – Open PIM
Select **Microsoft Entra Privileged Identity Management**.

![pim1](https://github.com/user-attachments/assets/b385093c-9d3d-4708-9e75-a92a4a42e268)


---

## 🔹 Step 5 – Go to Microsoft Entra Roles
Click **Microsoft Entra roles**.

![pim2](https://github.com/user-attachments/assets/023feff2-773b-447a-ac02-df65a2198eb8)


---

## 🔹 Step 6 – Open Roles
Click **Roles**.

![pim3](https://github.com/user-attachments/assets/ee9090a2-9965-45dc-be5b-84542112500e)


---

## 🔹 Step 7 – Add Assignment
Click **+ Add assignments**.

![pim4](https://github.com/user-attachments/assets/84c24125-c16b-48cc-82bb-50e497734757)


---

## 🔹 Step 8 – Select Role
Choose **User Administrator**.
![pim5](https://github.com/user-attachments/assets/e108f3f2-9fcc-4d57-b549-55b1ee739161)



---

## 🔹 Step 9 – Select Member
Click **Select members**.

![pim6](https://github.com/user-attachments/assets/4dd1424e-c8fc-499f-9e1c-11bfaa99b9f3)


---

## 🔹 Step 10 – Choose Adam Young
Select the user.

📸  
![Step 10](pim10.jpg)

---

## 🔹 Step 11 – Confirm Selection
Click **Select**.

📸  
![Step 11](pim11.jpg)

---

## 🔹 Step 12 – Continue
Click **Next**.

📸  
![Step 12](pim12.jpg)

---

## 🔹 Step 13 – Configure Assignment
- Set to **Eligible**
- Enable **Permanently eligible**

📸  
![Step 13](pim13.jpg)

---

## 🔹 Step 14 – Assign Role
Click **Assign**.

📸  
![Step 14](pim14.jpg)

---

# 🔐 Role Activation (User Perspective)

---

## 🔹 Step 15 – Sign in as Adam
Log in using Adam’s account.

📸  
![Step 15](pim15.jpg)

---

## 🔹 Step 16 – Stay Signed In
Click **Yes**.

📸  
![Step 16](pim16.jpg)

---

## 🔹 Step 17 – Additional Security Required
Click **Next** to continue setup.

📸  
![Step 17](pim17.jpg)

---

## 🔹 Step 18 – Install Authenticator
Download Microsoft Authenticator.

📸  
![Step 18](pim18.jpg)

---

## 🔹 Step 19 – Scan QR Code
Link account to Authenticator.

📸  
![Step 19](pim19.jpg)

---

## 🔹 Step 20 – Complete MFA Setup
Finish configuration.

📸  
![Step 20](pim20.jpg)

---

## 🔹 Step 21 – Activate Role
- Go to **My roles**
- Click **Activate**
- Enter reason (e.g., *User creation*)

📸  
![Step 21](pim21.jpg)

---

# ✅ Final Result
- Adam is assigned **Eligible User Administrator**
- MFA is enforced
- Role is activated **temporarily (JIT access)**

---

# 🔐 Security Concepts Demonstrated
- Least Privilege Access
- Just-In-Time (JIT) Administration
- Role-Based Access Control (RBAC)
- Multi-Factor Authentication (MFA)
- Identity Governance

---

# 💡 What I Learned
- PIM prevents permanent admin access and reduces risk
- MFA is required before privileged actions
- Eligible roles provide flexibility and security
- IAM focuses on controlled, temporary elevation

---

# 🚀 Why This Matters
This project demonstrates hands-on experience with:
- Microsoft Entra ID (Azure AD)
- Privileged Identity Management (PIM)
- Identity and Access Management (IAM)
- Real-world enterprise security practices
