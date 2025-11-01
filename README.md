# Optimizing-User-Group-and-Role-Management-with-Access-Control-and-Workflows

# 🧩 Optimizing User, Group, and Role Management with Access Control and Workflows

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

### **Step 2 – Create Groups**
- Groups created:
  - **Project Management Team**
  - **Development Team**

### **Step 3 – Create Roles**
- Defined two main roles:
  - `project_manager`
  - `team_member`

### **Step 4 – Assign Roles**
- **Alice** → `project_manager`, `u_project_table`, `u_task_table`  
- **Bob** → `team_member`, `u_task_table`

### **Step 5 – Assign Table Access**
- **Project Table** → accessible by *Project Manager*  
- **Task Table 2** → accessible by *Project Manager* and *Team Member*

### **Step 6 – Create ACL**
- Configured **4 ACLs** for table and field-level permissions:
  - Gave `team_member` access to **Task Table 2**
  - Provided edit access for **Comment** and **Status** fields

### **Step 7 – Create Flow in Flow Designer**
- Created a **Flow** that automatically assigns new **Operation Tickets** to the **Operations Group** upon creation.

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

