# Optimizing-User-Group-and-Role-Management-with-Access-Control-and-Workflows


This project is implemented on the **ServiceNow** platform to automate and optimize user, group, and role management operations.  
It also integrates **Access Control Lists (ACLs)** and **Flow Designer workflows** to ensure secure, structured, and efficient project management.

---

## 📘 Project Overview

In many organizations, managing user access and role permissions manually can lead to security gaps and inefficiencies.  
This project leverages **ServiceNow’s automation and access control capabilities** to create a robust, role-based management system with clearly defined workflows and permissions.

---

## 🎯 Objectives

- Automate creation and management of **Users**, **Groups**, and **Roles** in ServiceNow  
- Implement **Access Control Lists (ACLs)** for secure data access  
- Build workflows using **Flow Designer** for approval and task assignment  
- Establish **role-based access** to Project and Task tables  
- Improve collaboration and security through structured automation  

---

## ⚙️ System Requirements

### **Hardware**
- Processor: Intel i3 or higher  
- RAM: Minimum 4 GB  
- Storage: 100 MB of free disk space  
- Internet Connection: Required  

### **Software**
- Platform: ServiceNow Personal Developer Instance  
- Browser: Google Chrome or Microsoft Edge  
- Scripting: JavaScript (Business Rules & Flow Designer)

---

## 🧠 Methodology

### **Step 1 – Create Users**
- Created two users:
  - **Alice (Project Manager)**
  - **Bob (Team Member)**
 
    ![1 png](https://github.com/user-attachments/assets/0d434e59-45cc-4690-86fa-b2c69ca2c1c9)


### **Step 2 – Create Groups**
- Groups created:
  - **Project Management Team**
  - **Development Team**
 
    <img width="1809" height="790" alt="2 png" src="https://github.com/user-attachments/assets/0ef42086-7f36-4a41-9627-0f2d96a5fc53" />


### **Step 3 – Create Roles**
- Defined two main roles:
  - `project_manager`
  - `team_member`

  <img width="1809" height="821" alt="3 png" src="https://github.com/user-attachments/assets/31cb450d-e4b3-460b-994d-591ae0e6f1dd" />


### **Step 4 – Assign Roles**
- **Alice** → `project_manager`, `u_project_table`, `u_task_table`  
- **Bob** → `team_member`, `u_task_table`

  <img width="1805" height="808" alt="image" src="https://github.com/user-attachments/assets/e21ccaab-5a82-458a-b6ae-9eb9ff2eed25" />


### **Step 5 – Assign Table Access**
- **Project Table** → accessible by *Project Manager*  
- **Task Table 2** → accessible by *Project Manager* and *Team Member*

  <img width="1814" height="796" alt="image" src="https://github.com/user-attachments/assets/43d7dd75-42ae-4f77-b3e6-aa2b992971f1" />


### **Step 6 – Create ACL**
- Configured **4 ACLs** for table and field-level permissions:
  - Gave `team_member` access to **Task Table 2**
  - Provided edit access for **Comment** and **Status** fields
 
    <img width="1810" height="532" alt="image" src="https://github.com/user-attachments/assets/ea020403-64b9-4b6a-9e9c-5fba0fe544e2" />


### **Step 7 – Create Flow in Flow Designer**
- Created a **Flow** that automatically assigns new **Operation Tickets** to the **Operations Group** upon creation.

  <img width="1814" height="862" alt="image" src="https://github.com/user-attachments/assets/d80db307-5671-4550-a74e-76c6d6d553c9" />


---

## 💡 Results & Discussion

- Automated user, group, and role management successfully  
- Role-based access and ACLs worked as intended  
- **Flow Designer** ensured automatic ticket assignment to the correct group  
- Reduced manual errors and improved collaboration between team members  

---


🎥project demo
https://drive.google.com/file/d/12_SvK6GYURYAER9wQak7gqO-me4O2sXd/view?usp=drive_link

Acknowledgement

This project was completed under the Muthalvan Program as part of academic learning at Grace College of Engineering, Thoothukudi. Special thanks to mentors and the ServiceNow Developer Community for guidance and support.

👨‍💻 Author
Team Leader : Jeffrin S

Team member : Deepika G

Team member : Hinduja M

Team member : Muthuselvi S

department : AI-DS 
College: Grace College of Engineering, Thoothukudi

## 🏁 Conclusion

This project demonstrates a structured approach to user and access management in ServiceNow.  
With clear roles for **Alice** (Project Manager) and **Bob** (Team Member), the workflow promotes accountability, communication, and efficiency.  
The integration of ACLs and automation workflows ensures both **security** and **productivity** in organizational environments.

---

## 📂 Folder Structure

