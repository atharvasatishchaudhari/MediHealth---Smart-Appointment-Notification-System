

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

```bash
📦 MediHealth
├── backend
│   ├── config
│   │   └── db.js
│   ├── middleware
│   │   ├── auth.js
│   │   └── isDoctor.js
│   ├── models
│   │   ├── Appointment.js
│   │   ├── Doctor.js
│   │   └── User.js
│   ├── routes
│   │   ├── appointments.js
│   │   ├── auth.js
│   │   └── doctors.js
│   ├── node_modules
│   ├── .env
│   ├── package.json
│   ├── package-lock.json
│   ├── seedDoctors.js
│   ├── server.js
│   └── socket.js
│
├── medi-booking (frontend)
│   ├── public
│   │   └── vite.svg
│   ├── src
│   │   ├── assets
│   │   ├── components
│   │   ├── context
│   │   ├── pages
│   │   ├── api.js
│   │   ├── App.css
│   │   ├── App.jsx
│   │   ├── index.css
│   │   ├── main.jsx
│   │   └── socket.js
│   ├── .gitignore
│   ├── eslint.config.js
│   ├── index.html
│   ├── package.json
│   ├── package-lock.json
│   ├── vite.config.js
│   └── README.md
















