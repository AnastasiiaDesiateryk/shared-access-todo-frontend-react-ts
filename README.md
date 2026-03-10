# 📝 To-Do List Application — Requirements Document  
**Project:** Internal Productivity Tool (MVP)  
**Author:** Anastasiia Desiateryk  
**Date:** 2025-10-04  

---

## 1. Functional Requirements  

### 1.1 Task Management  
- Create a new task with attributes:  
  - **Title** (mandatory)  
  - **Description** (optional)  
  - **Due date** (optional)  
  - **Priority** (Low / Medium / High)  
- Edit or delete existing tasks.  
- Mark a task as **completed**.  
- Filter tasks by **status** (open/completed), **priority**, or **hashtag/category**.  

### 1.2 User Account  
- Simple authentication.  
- Each user sees **only their own tasks** (no shared boards in MVP).  

### 1.3 Task Organization  
- Display tasks in a **structured list**, sorted by **due date** or **priority**.  
- Support **search** by task title, hashtag, or category.  

### 1.4 Persistence  
- All tasks are stored in a **secure database**.  
- Data remains available **after logout/login**.  

---

## 2. Non-Functional Requirements  

### 2.1 Performance  
- The system must load the user’s task list within **2 seconds** (for up to 200 tasks).  

### 2.2 Security & Compliance  
- Passwords stored using **strong hashing** (e.g., bcrypt).  
- **Data at rest** encrypted.  
- **Data in transit** encrypted.  
- Authentication tokens expire after **24 hours** of inactivity.  

### 2.3 Usability  
- Interface must be **mobile-first**, responsive on desktop and mobile browsers.  

### 2.4 Auditability  
- Changes to tasks (**create/update/delete/complete**) must be **logged** with timestamp and user ID.  

---

## 3. Constraints  

 

### 3.1 Budget  
- Limited to **internal resources** (no external vendor costs).  

### 3.2 Technology  
- **Backend:** PostgreSQL, Java  
- **Frontend:** React (Vite)  
- **Deployment:** Render  
- **Testing:** Jacoco

---

## 4. Open Questions  
- Should the MVP support **shared task lists** for teams, or remain individual?  
- Should **notifications/reminders** be included in the initial scope?  
- What is the **maximum number of users** expected for the pilot phase?  

---
### Traceability
- Linked to [User Stories](./docs/3_UserStories.md)
- Linked to [Use Case Diagram](./docs/4_UseCaseDiagram.md)
  
© 2025 Anastasiia Desiateryk — Internal Project Documentation

## Running the code

Run `npm i` to install the dependencies.

Run `npm run dev` to start the development server.
