# 🏥 Hospital Management System (HMS)

The **Hospital Management System (HMS)** is a **Spring Boot and React.js-based full-stack application** designed to automate hospital operations including patient management, staff administration, billing, and inventory workflows. It enhances efficiency, security, and scalability through modern software architecture.

---

<h2>🎥 Project Demo</h2>

<p align="center">
  <a href="https://www.youtube.com/watch?v=qwYNyGy0JGU" target="_blank">
    <img src="https://img.youtube.com/vi/qwYNyGy0JGU/0.jpg" 
         alt="Hospital Management System Demo Video" 
         width="70%" style="border-radius:10px;">
  </a>
</p>


## 📚 Table of Contents

- [Overview](#overview)
- [Modules](#modules)
- [User Roles](#user-roles)
- [Authentication & Authorization](#authentication--authorization)
- [Core Functionalities](#core-functionalities)
- [Billing & Payments](#billing--payments)
- [Inventory & Medicine Management](#inventory--medicine-management)
- [Database Design](#database-design)
- [Tech Stack](#tech-stack)
- [Installation](#installation)
- [Contributors](#contributors)

---

## 📖 Overview

Developed a full-stack Hospital Management System using **Spring Boot**, **React.js**, and **MySQL** to automate patient, staff, billing, and inventory workflows.

### Key Highlights
- Role-based access control (**Admin**, **Doctor**, **Patient**, **Receptionist**, **Accountant**) with **JWT-secured RESTful APIs**.  
- Enhanced query performance and operational efficiency by **40%** using **Spring Data JPA**, **Swagger**, and optimized database design.  
- Containerized deployment using **Docker** ensuring scalability, data privacy, and transactional integrity with **Spring Security**.  
- Automated reporting and alert notifications for real-time operations.

---

## 📦 Modules

- **Admin Module** – Manage departments, users, wards, and inventory.
- **Patient Module** – Register, view medical history, prescriptions, and billing status.
- **Doctor Module** – Manage appointments, create prescriptions, and track patient progress.
- **Receptionist Module** – Handle patient admissions, discharges, and scheduling.
- **Accountant Module** – Generate and manage invoices and payment records.

---

## 👥 User Roles

### 🧑‍💼 Admin
- Manage hospital resources: doctors, patients, staff, medicines, and wards.
- Monitor hospital activity and analytics.

### 🩺 Doctor
- Access assigned patients and update their medical records.
- Issue prescriptions and treatment plans.

### 👨‍🦱 Patient
- Book appointments and view medical records.
- Access discharge summary and billing details.

### 💁 Receptionist
- Register new patients and assign doctors/wards.
- Manage admission and discharge workflows.

### 💰 Accountant
- Generate invoices and track transactions.
- Manage and update payment statuses.

---

## 🔐 Authentication & Authorization

- **JWT-based Security** for login and API access.
- **Role-based Authorization** to ensure secure and restricted data access.
- **Swagger UI** for API testing and documentation.

### Key Endpoints:
- `POST /auth/signup` – Register new users  
- `POST /auth/login` – Authenticate user and issue JWT  
- `POST /auth/refresh` – Refresh expired access tokens  

---

## ⚙️ Core Functionalities

- **Patient Management** – Registration, appointment scheduling, and medical record maintenance.
- **Staff Management** – Add, update, or remove hospital employees and assign roles.
- **Ward Management** – Allocate and monitor room/bed availability.
- **Prescription Handling** – Doctors issue prescriptions linked to patients and medications.
- **Alerts & Notifications** – Success/error popups for user feedback on CRUD operations.

---

## 💳 Billing & Payments

- Automated **invoice generation** for every patient discharge.
- Real-time **billing summary** for treatments, medicines, and room stays.
- Option to download invoices in **PDF format**.
- Tracks all transaction records for accounting integrity.

---

## 💊 Inventory & Medicine Management

- Add and update medicines in stock.
- Automatic alerts for low-stock medicines.
- Assign prescribed medicines to specific patients.
- Track ward/bed availability dynamically.

---

## 🗄️ Database Design

The HMS uses a **relational database (MySQL)** with well-normalized tables:

| Table | Description |
|--------|--------------|
| `users` | Stores login credentials and roles |
| `employees` | Holds hospital staff information |
| `patients` | Maintains patient medical and personal records |
| `wards` | Tracks bed availability and charges |
| `doctors` | Stores doctor details and consultation charges |
| `medicines` | Medicine inventory |
| `medicines_assigned` | Mapping between prescribed medicines and patients |
| `doctor_visits` | Logs doctor-patient visits and prescriptions |

---

## 🧠 Tech Stack

**Backend:**
- Java 21  
- Spring Boot 3  
- Spring Security (JWT)  
- Spring Data JPA  
- Swagger (API Documentation)

**Frontend:**
- React.js  
- HTML, CSS, JavaScript  

**Database:**
- MySQL  

**DevOps:**
- Docker  
- Git, GitHub  

---

## ⚙️ Installation

### Prerequisites:
- Java 17 or above  
- React.js
- Spring Boot  
- MySQL Server  
- Docker (optional)

### Steps:
1. Clone the repository:
   ```bash
   git clone https://github.com/Ankitmittal0610/Hospital_Management_System.git
   cd Hospital_Management_System
   ```
2. Setup database in MySQL and update credentials in application.properties.
3. Run backend:
   ```bash
   mvn spring-boot:run
   ```
5. Navigate to frontend directory and start the React app:
   ```bash
   npm install
   npm start
   ```
## 📌 Contributors

**Developed by:** Ankit Mittal 
- **Connect:** [LinkedIn](https://www.linkedin.com/in/ankitmittal6949)

---
