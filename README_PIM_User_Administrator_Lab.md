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





---

## 🔹 Step 14 – Assign Role
Click **Assign**.

![pim9](https://github.com/user-attachments/assets/f87e6500-44ee-429d-9dda-a35e9433532c)



---

# 🔐 Role Activation (User Perspective)

---

## 🔹 Step 15 – Sign in as Adam

Log in using Adam Young’s account.

![pim10](https://github.com/user-attachments/assets/70501e67-dd7a-4d34-a737-432876d7d089)

---

## 🔹 Step 16 – Navigate to Privileged Identity Management (PIM)

* Go to **All Services**
* Search for **Entra**
* Select **Microsoft Entra Privileged Identity Management**

![pim11](https://github.com/user-attachments/assets/db0f8e52-ec22-41dc-9099-d0b69594c2d9)

---

## 🔹 Step 17 – Open My Roles

* Click **My roles** under the PIM menu

![pim12](https://github.com/user-attachments/assets/7181c1ff-b730-453d-8140-c785de53c334)

---

## 🔹 Step 18 – View Eligible Roles

* Under **Eligible assignments**, locate:

  * **User Administrator**

---

## 🔹 Step 19 – Activate Role

* Click **Activate** next to the role

---

## 🔹 Step 20 – Additional Verification Required (MFA Triggered)

* A prompt will appear: **“Additional verification required”**
* Click to continue

👉 This is where MFA is enforced (NOT during initial login)

---

## 🔹 Step 21 – Set Up Microsoft Authenticator

* Install the **Microsoft Authenticator app**
* Scan the QR code
* Complete the setup

---

## 🔹 Step 22 – Enter Activation Details

* Set **Duration** (default: 8 hours)
* Enter a reason (example: *User creation*)

---

## 🔹 Step 23 – Activate Role

* Click **Activate**

---

# ✅ Final Result

* Adam is assigned **Eligible User Administrator**
* MFA is enforced during role activation via PIM
* Role is activated temporarily (**Just-In-Time access**)

---

# 🔐 Security Concepts Demonstrated

* Least Privilege Access
* Just-In-Time (JIT) Administration
* Role-Based Access Control (RBAC)
* Multi-Factor Authentication (MFA)
* Identity Governance

---

# 💡 What I Learned

* PIM reduces risk by eliminating permanent admin access
* MFA is enforced when elevating privileges, not just at login
* Eligible roles provide secure, temporary access
* IAM focuses on controlled privilege escalation

---

# 🚀 Why This Matters (Recruiters)

This project demonstrates hands-on experience with:

* Microsoft Entra ID (Azure AD)
* Privileged Identity Management (PIM)
* Identity & Access Management (IAM)
* Enterprise security best practices
