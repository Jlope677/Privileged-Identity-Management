# 🔐 Azure IAM Lab: Privileged Identity Management (PIM) – Just-In-Time Role Activation

---

## 📌 Overview
This lab demonstrates the implementation of Microsoft Entra Privileged Identity Management (PIM) to control and secure privileged access using a Just-In-Time (JIT) model.

In this project, I:
- Assigned a user (Adam Young) with eligible access to the User Administrator role  
- Enforced multi-factor authentication (MFA) during role activation  
- Validated temporary privilege elevation through PIM  

This approach aligns with modern Identity and Access Management (IAM) and Zero Trust security principles by minimizing standing administrative access.

---

## 🎯 Objectives
- Implement Privileged Identity Management (PIM) in Microsoft Entra ID  
- Assign eligible (non-permanent) administrative access  
- Enforce MFA during privilege elevation  
- Activate roles using Just-In-Time (JIT) access  
- Apply least privilege and identity governance best practices  

---

## 🧱 Environment & Technologies
- Microsoft Azure Portal  
- Microsoft Entra ID  
- Privileged Identity Management (PIM)  
- Microsoft Authenticator (MFA)  
- Role-Based Access Control (RBAC)  

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
![pim12](https://github.com/user-attachments/assets/7181c1ff-b730-453d-8140-c785de53c334)

---

## 🔹 Step 17 – Open My Roles

* Click **My roles** under the PIM menu

![pim13](https://github.com/user-attachments/assets/2a102b13-afb6-4112-9a1a-00032c89a718)


---

## 🔹 Step 18 – View Eligible Roles

* Under **Eligible assignments**, locate:

  * **User Administrator**

---

## 🔹 Step 19 – Activate Role

* Click **Activate** next to the role

![pim14](https://github.com/user-attachments/assets/50cb11d3-fe5f-493e-8c10-a91fb4ebf60e)

---

## 🔹 Step 20 – Additional Verification Required (MFA Triggered)

* A prompt will appear: **“Additional verification required”**
* Click to continue

👉 This is where MFA is enforced (NOT during initial login)

![pim15](https://github.com/user-attachments/assets/520d5852-f76c-4018-8441-c36f4acdddf0)

---

## 🔹 Step 21 – Set Up Microsoft Authenticator

* Install the **Microsoft Authenticator app**
* Scan the QR code
* Complete the setup

![pim16](https://github.com/user-attachments/assets/0d11aaa6-b3a2-4851-bf07-9aa38f9e4abe)
![pim17](https://github.com/user-attachments/assets/43d1c179-b28f-4e70-92b4-5cc9e4d89598)
![pim18](https://github.com/user-attachments/assets/5ee7fb5e-cb42-4f75-be7b-f274c5490ed3)
![pim19](https://github.com/user-attachments/assets/d070a96f-a377-4319-b210-b7123359220f)
![pim20](https://github.com/user-attachments/assets/f37e410a-b20e-430c-b561-950cc1e081ee)





---

## 🔹 Step 22 – Enter Activation Details

* Set **Duration** (default: 8 hours)
* Enter a reason (example: *User creation*)


---

## 🔹 Step 23 – Activate Role

* Click **Activate**

![pim21](https://github.com/user-attachments/assets/4f2b343f-6f06-4852-9420-452c9511daa8)

---

## ✅ Results
- User successfully assigned eligible administrative access  
- MFA enforced during role activation  
- Role activated using Just-In-Time (JIT) access  
- No permanent privileged access granted  

---

## 🔐 Security Concepts Demonstrated
- Least Privilege Access  
- Just-In-Time (JIT) Administration  
- Role-Based Access Control (RBAC)  
- Multi-Factor Authentication (MFA)  
- Identity Governance  

---

## 💡 Key Takeaways
- PIM reduces risk by eliminating permanent administrative access  
- MFA tied to privilege elevation adds an additional layer of security  
- Eligible role assignments provide flexibility without compromising security  
- This model is commonly used in enterprise IAM and Zero Trust environments  

---

## 🚀 Why This Project Matters
This project demonstrates hands-on experience with:
- Microsoft Entra ID administration  
- Privileged Identity Management (PIM)  
- Secure role assignment and activation workflows  
- Enterprise identity security controls  

---

## 🔄 Next Steps
- Implement PIM approval workflows  
- Configure Conditional Access policies  
- Explore Access Reviews and Identity Governance  
- Automate role assignments using PowerShell or Azure CLI  

---
