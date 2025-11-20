# 🚀 Full Stack CRUD Application — React + Spring Boot + MySQL

This is a full-stack CRUD (Create, Read, Update, Delete) application built using:

- **Frontend:** React + Axios + Bootstrap  
- **Backend:** Spring Boot + Spring Web + Spring Data JPA  
- **Database:** MySQL  


## 📁 Project Structure

fullstack-react-springboot/
│
├── react-frontend/ # React Application
│ ├── src/
│ ├── public/
│ └── package.json
│
└── springboot-backend/ # Spring Boot REST API
├── src/main/java/
├── src/main/resources/
└── pom.xml

---

## 🛠 Tech Stack

### Frontend
- React
- React Router
- Axios
- Bootstrap 5

### Backend
- Spring Boot
- Spring Web
- Spring Data JPA
- MySQL Driver

---

## 📦 Features

### ✔ User Management
- Add a user  
- View user details  
- Edit user  
- Delete user  
- View all users  

### ✔ REST API Endpoints

| Method | Endpoint         | Description          |
|--------|------------------|----------------------|
| GET    | `/users`        | Get all users        |
| GET    | `/user/{id}`    | Get user by ID       |
| POST   | `/user`         | Add a new user       |
| PUT    | `/user/{id}`    | Update existing user |
| DELETE | `/user/{id}`    | Delete user          |

---

## ⚙️ Backend — How to Run

### 1️⃣ Configure MySQL  
Edit:  
`springboot-backend/src/main/resources/application.properties`

spring.datasource.url=jdbc:mysql://localhost:3306/YOUR_DB_NAME
spring.datasource.username=YOUR_USERNAME
spring.datasource.password=YOUR_PASSWORD
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true



### 2️⃣ Start Backend


cd springboot-backend
mvn spring-boot:run
API will run at:


http://localhost:8080
🎨 Frontend — How to Run
1️⃣ Install dependencies

cd react-frontend
npm install
2️⃣ Start frontend

npm start
App will run at:


http://localhost:3000
🔗 Connecting Frontend & Backend
Axios request example:


await axios.post("http://localhost:8080/user", user);
Enable CORS in Spring Boot:


@CrossOrigin("http://localhost:3000")
🗄 Database Schema (Auto-Generated)
Column	Type	Description
id	BIGINT PK	Auto-increment ID
name	VARCHAR	User's Name
username	VARCHAR	Username
email	VARCHAR	Email Address


🤝 Contributing
Pull requests are welcome. For major changes, open an issue first.

📝 License
Free to use and modify.
