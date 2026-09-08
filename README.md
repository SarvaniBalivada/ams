# 🏃 Athlete Management System (AMS)

A full-stack **Athlete Management System** designed to digitally manage athletes, coaches, training activities, and competitions through a centralized web application.

The system provides separate modules for managing athlete and coach information, training sessions, competitions, and user authentication.

## 🚀 Features

### 🔐 Authentication & Authorization

* User registration and login
* JWT-based authentication
* Password encryption
* Role-based user registration for athletes and coaches
* Protected backend APIs

### 🏃 Athlete Management

* Add athlete details
* View athlete information
* Update athlete information
* Delete athlete records
* Manage athlete profiles

### 👨‍🏫 Coach Management

* Add and manage coach information
* View coach details
* Update coach records
* Delete coach records

### 🏋️ Training Management

* Create and manage training activities
* View training information
* Update and delete training records
* Manage athlete training-related data

### 🏆 Competition Management

* Add competition information
* View competition details
* Update competition records
* Delete competition records

### 📊 Dashboard

* Centralized interface for accessing different modules
* Navigation between athlete, coach, training, and competition management

---

## 🛠️ Tech Stack

### Frontend

* **React.js**
* **Vite**
* **JavaScript**
* **Axios**
* HTML5
* CSS3

### Backend

* **Java**
* **Spring Boot**
* **Spring Security**
* **JWT**
* **Spring Data JPA**
* REST APIs

### Database

* **MySQL**

### Development Tools

* Git
* GitHub
* VS Code / IntelliJ IDEA

---

## 🏗️ System Architecture

The application follows a layered full-stack architecture:

```text
                ┌──────────────────────┐
                │    React Frontend    │
                │      (Vite)          │
                └──────────┬───────────┘
                           │
                    Axios / REST API
                           │
                           ▼
                ┌──────────────────────┐
                │ Spring Boot Backend  │
                └──────────┬───────────┘
                           │
                  ┌────────┴────────┐
                  │                 │
                  ▼                 ▼
            Controllers         Security
                  │             + JWT
                  ▼
              Services
                  │
                  ▼
            Repositories
                  │
                  ▼
              Database
```

The backend is organized into separate **Controller, Service, Repository, Entity, DTO, and Authentication/Security** layers.

---

## 📂 Project Structure

```text
AMS
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   │   ├── Athlete/
│   │   │   ├── Coach/
│   │   │   ├── Competition/
│   │   │   ├── Training/
│   │   │   ├── Dashboard/
│   │   │   └── Authentication/
│   │   │
│   │   ├── services/
│   │   │   ├── AthleteService
│   │   │   ├── AuthService
│   │   │   ├── CoachService
│   │   │   ├── CompetitionService
│   │   │   └── TrainingService
│   │   │
│   │   └── ...
│   │
│   └── package.json
│
└── backend/
    └── src/
        └── main/
            └── java/
                └── springboot_based/
                    └── ams/
                        ├── controller/
                        ├── service/
                        ├── repository/
                        ├── entity/
                        ├── dto/
                        ├── auth/
                        └── security/
```

---

## 🔄 Application Workflow

1. The user registers or logs into the application.
2. The backend authenticates the user using **Spring Security**.
3. A **JWT token** is generated after successful authentication.
4. The frontend uses the token when accessing protected APIs.
5. Users can access the available modules based on the application flow.
6. React communicates with the Spring Boot backend using REST APIs.
7. Spring Boot processes the request through the Controller and Service layers.
8. Spring Data JPA communicates with the database through the Repository layer.
9. The response is returned to the React frontend and displayed to the user.

---

## 🔑 Authentication Flow

```text
User
  │
  ▼
Login / Registration
  │
  ▼
React Frontend
  │
  ▼
Spring Boot Authentication API
  │
  ▼
Spring Security
  │
  ▼
Credentials Verification
  │
  ▼
JWT Generation
  │
  ▼
JWT Token
  │
  ▼
React Frontend
  │
  ▼
Authenticated API Requests
```

JWT-based authentication helps secure the backend APIs and prevents unauthorized access to protected resources.

---

## 📡 REST API Modules

The backend provides REST APIs for the major application modules:

| Module         | Operations                   |
| -------------- | ---------------------------- |
| Authentication | Register, Login              |
| Athletes       | Create, Read, Update, Delete |
| Coaches        | Create, Read, Update, Delete |
| Training       | Create, Read, Update, Delete |
| Competitions   | Create, Read, Update, Delete |

---

## 💡 Key Learning Outcomes

Through this project, I gained practical experience in:

* Developing a full-stack web application
* Building REST APIs using Spring Boot
* Developing reusable UI components using React
* Connecting React with a Spring Boot backend
* Implementing CRUD operations
* Working with Spring Data JPA
* Implementing JWT-based authentication
* Structuring applications using layered architecture
* Working with frontend-backend API integration
* Using Git and GitHub for version control

---

## 🔮 Future Improvements

Some possible future enhancements include:

* Advanced role-based access control
* Athlete performance analytics and visualization
* Training progress tracking
* Competition performance reports
* Notifications and reminders
* Advanced search and filtering
* Cloud deployment and scalability improvements

---

## 👨‍💻 Author

**Sai Sarvani Balivada**

B.Tech – Computer Science and Engineering

GitHub: [SarvaniBalivada](https://github.com/SarvaniBalivada)

---

## 📄 License

This project is developed for educational and learning purposes.
