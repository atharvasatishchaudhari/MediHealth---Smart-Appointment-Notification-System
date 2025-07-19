

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
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/931736c8-5c2b-4b8f-bfc8-3bd630570358" />

<img width="1919" height="825" alt="image" src="https://github.com/user-attachments/assets/e3359522-f08a-4c68-88e7-1c0088fa74e4" />

<img width="1919" height="900" alt="image" src="https://github.com/user-attachments/assets/ae03053f-3e7f-4a53-8570-c96be5782dbe" />

<img width="1905" height="825" alt="image" src="https://github.com/user-attachments/assets/64710a47-78ff-4574-94ec-f43619c414a9" />

<img width="1913" height="823" alt="image" src="https://github.com/user-attachments/assets/d5bb05c2-450b-4e2e-9017-c14687faa4a5" />


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

















