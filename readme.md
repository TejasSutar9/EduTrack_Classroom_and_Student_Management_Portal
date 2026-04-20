# 🎓 EduTrack – Classroom & Student Management Portal

Java • Spring Boot • MongoDB • Maven

---

## 🔹 Overview

EduTrack is a backend application built using Spring Boot and MongoDB to manage classroom batches efficiently.

It provides REST APIs for performing CRUD operations on batch data and ensures structured backend architecture. This project is backend-focused and can be integrated with any frontend framework like React, Angular, or Vue.

---

## 🛠 Technology Stack

| Layer      | Technology        |
| ---------- | ----------------- |
| Backend    | Java, Spring Boot |
| Database   | MongoDB           |
| Build Tool | Maven             |
| Testing    | Postman           |
| IDE        | IntelliJ IDEA     |
| Java       | 17+               |

---

## 📂 Project Structure

```
src/main/java/com/edutrack/portal
├── Controller/
│   ├── BatchEntryController.java
│   └── HealthCheck.java
├── Entity/
│   └── BatchEntry.java
├── Repository/
│   └── BatchEntryRepository.java
├── Service/
│   └── BatchEntryService.java
└── EduTrackApplication.java

src/main/resources/
└── application.properties

pom.xml
.gitignore
```

---

## 🚀 Features

* CRUD operations for managing classroom batches
* MongoDB integration for reliable data storage
* RESTful APIs for easy frontend integration
* Layered architecture (Controller → Service → Repository)
* Health check API for application status

---

## 📌 API Endpoints

| Method | Endpoint          | Description              |
| ------ | ----------------- | ------------------------ |
| GET    | /api/batches      | Get all batches          |
| POST   | /api/batches      | Create new batch         |
| PUT    | /api/batches/{id} | Update batch             |
| DELETE | /api/batches/{id} | Delete batch             |
| GET    | /health           | Check application status |

---

## ⚙️ Installation & Run

### 1. Clone Repository

```
git clone https://github.com/your-username/your-repo-name.git
cd EduTrack
```

---

### 2. Configure MongoDB

* Ensure MongoDB is running on default port **27017**
* Database will be created automatically

---

### 3. Run Project

```
mvn clean install
mvn spring-boot:run
```

---

### 4. Test APIs

Use Postman or browser

Base URL:

```
http://localhost:8080/api/batches
```

Example JSON:

```
{
  "name": "Java Full Stack",
  "fees": 5000
}
```

---

## 📈 Future Enhancements

* Add student management module
* Implement validation and exception handling
* Add authentication (Spring Security)
* Build frontend UI

---

## 👨‍💻 Author

**Tejas Pradip Sutar**

---

## ⭐ Conclusion

EduTrack demonstrates how to build a structured backend system using Spring Boot and MongoDB for managing classroom batches efficiently.
