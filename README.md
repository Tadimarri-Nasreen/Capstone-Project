# 🚌 Capstone Project: Bus Reservation System  

A **full-stack Bus Reservation System** developed as my **Capstone Project**.  
It allows **users** to register, search for buses, book tickets, and manage reservations, while **admins** can manage buses and bookings.  

---

## 🚀 Tech Stack
- **Frontend**: React.js, Axios, React Router, Bootstrap  
- **Backend**: Java, Spring Boot, Spring Data JPA, Spring Security (JWT)  
- **Database**: MySQL (Production) / H2 (Development)  
- **Build Tools**: Maven, npm  

---

## ✨ Features  

### 👤 User  
- Register & Login with JWT Authentication  
- Search buses by source, destination, and date  
- Book tickets and view booking history  
- Cancel bookings  

### 👨‍💼 Admin  
- Add, update, or delete buses  
- View and manage all bookings  
- Manage passengers  

---

## 📂 Project Structure

bus-reservation-system/
├── backend/   (Spring Boot backend) Runs on: http://localhost:8080
└── frontend/  (React.js frontend)   Runs on: http://localhost:3000

---

## 🎯 How to Run
1. Start **backend** (`8080`).  
2. Start **frontend** (`3000`).  
3. Open (http://localhost:3000).  
4. Register → Login → Search buses → Book tickets.  

---

## 🔑 Authentication  

The system uses **JWT (JSON Web Token)** for authentication.  

### 📌 Register User  
**POST** `http://localhost:8080/api/user/register`  

```json
{
  "name": "John Doe",
  "email": "user@example.com",
  "password": "User@123",
  "roles": "PASSENGER",
  "gender": "Male",
  "contact": "9999999999",
  "street": "1st Street",
  "city": "City",
  "pincode": "123456"
}

---

## 📌 Login User  

**POST** `http://localhost:8080/api/user/login`  

```json
{
  "emailId": "user@example.com",
  "password": "User@123",
  "role": "PASSENGER"
}

✅ On successful login, you will receive a **JWT Token**:  

```json
{
  "jwtToken": "eyJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJ1c2VyQGVtYWlsLmNvbSIsImlhdCI6MTc1NjIwMDgyNiwiZXhwIjoxNzU2ODEwMDYwfQ.KUZCJW90185NHvY301WCuWPYaM2WaKMJmKMU-qvSNY",
  "success": true
}

## 📜 This project is created as part of my **Capstone Project** for learning and educational purposes.  
