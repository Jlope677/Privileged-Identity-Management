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




---

## 🔹 Step 11 – Confirm Selection
Click **Select**.

![pim7](https://github.com/user-attachments/assets/adb78a95-0756-4712-a568-5e36faf20f15)



---

## 🔹 Step 12 – Continue
Click **Next**.

![pim8](https://github.com/user-attachments/assets/230fe53b-a9d7-41bc-bc65-a425b063b6fe)



---

## 🔹 Step 13 – Configure Assignment
- Set to **Eligible**
- Enable **Permanently eligible**
![pim9](https://github.com/user-attachments/assets/f87e6500-44ee-429d-9dda-a35e9433532c)




---

## 🔹 Step 14 – Assign Role
Click **Assign**.




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
