

# 🏥 MediHealth – Smart Appointment & Notification System

MediHealth is a full-stack healthcare appointment booking system that enables **patients to book appointments** with doctors, **doctors to manage schedules**, and supports **real-time updates** for appointment cancellations. The system handles **emergency delays**, **authentication**, and **real-time slot availability notifications** using `Socket.IO`.

---

## 🚀 Features

### 🔐 Authentication
- JWT-based login/signup for both patients and doctors.
- Role-based access control (doctor vs. patient).

### 🗓️ Appointment Booking
- Patients can:
  - Book appointments by department, doctor, date & time.
  - Cancel their bookings.
- Doctors can:
  - View all their appointments.
  - Reschedule or delay appointments in emergency.

### 📡 Real-time Notifications (Socket.IO)
- When a patient cancels an appointment:
  - All other users receive real-time alerts for the newly available slot.

### 🆘 Emergency Delay Handler
- Doctors can shift all upcoming appointments forward by a delay (in minutes).

---

## ⚙️ Tech Stack

### 🖥 Frontend
- **React.js**
- **Context API** for authentication state
- **Axios** for API calls
- **Socket.IO Client** for real-time communication

### 🌐 Backend
- **Node.js + Express**
- **MongoDB (Mongoose)**
- **Socket.IO Server**
- **JWT** for user authentication
- **Dotenv** for environment configuration

---

## 📁 Folder Structure
📦 MediHealth
<img width="247" height="806" alt="image" src="https://github.com/user-attachments/assets/df967f67-fc5c-4566-9f1d-d9ee9fbf336f" />
<img width="252" height="784" alt="image" src="https://github.com/user-attachments/assets/54fde455-9370-4f66-b7e9-99a613fa2913" />
















