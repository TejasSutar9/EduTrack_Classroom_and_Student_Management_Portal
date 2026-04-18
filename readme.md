# 🎓 EduTrack – Classroom & Student Management Portal

Java • Spring Boot • MongoDB • Maven

---

## 🔹 Overview

EduTrack is a backend system built with **Spring Boot** and **MongoDB** to manage classrooms and student batches efficiently.

It provides REST APIs for CRUD operations and ensures:

* Data validation
* Exception handling
* Clean JSON responses

This project is **backend-only** and designed for integration with any frontend (React / Angular / Vue).

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
EduTrack/
├── src/main/java/com/edutrack
│   ├── config/                  
│   │   └── MongoConfig.java
│   ├── controller/              
│   │   └── BatchEntryController.java
│   ├── entity/                  
│   │   └── BatchEntry.java
│   ├── exception/               
│   │   ├── ResourceNotFoundException.java
│   │   └── GlobalExceptionHandler.java
│   ├── repository/              
│   │   └── BatchEntryRepository.java
│   ├── service/                 
│   │   └── BatchEntryService.java
│   └── EduTrackApplication.java 
├── src/main/resources/
│   └── application.properties   
├── pom.xml                      
└── .gitignore
```

---

## 🚀 Features

* CRUD operations for Classroom/Batches
* MongoDB integration for persistent storage
* RESTful APIs for easy frontend integration
* Global Exception Handling for clean error responses
* Validation to prevent empty names or negative fees

---

## 📌 API Endpoints

| Method | Endpoint               | Description          |
| ------ | ---------------------- | -------------------- |
| GET    | `/api/batches`         | Get all batches      |
| POST   | `/api/batches`         | Create a new batch   |
| PUT    | `/api/batches/id/{id}` | Update a batch by ID |
| DELETE | `/api/batches/id/{id}` | Delete a batch by ID |
| DELETE | `/api/batches/all`     | Delete all batches   |

✔ All endpoints return JSON responses with proper HTTP status codes.

---

## ⚙️ Installation & Run

### 1. Clone the repository

```
git clone https://github.com/YourUsername/edutrack-strudent-and-classroom-management.git
cd edutrack-strudent-and-classroom-management/EduTrack
```

---

### 2. Configure MongoDB

* Make sure MongoDB is running locally (default port: **27017**)
* Database **edutrack** will be created automatically

---

### 3. Build & Run

```
mvn clean install
mvn spring-boot:run
```

---

### 4. Test APIs

Use Postman or any REST client

Base URL:

```
http://localhost:8080/api/batches
```

### Example POST Request

```
{
  "name": "Java Full Stack",
  "fees": 5000
}
```

---

## 💡 Validation & Error Handling

* Name cannot be empty
* Fees must be positive
* Invalid ID → 404 Not Found

### Example Error Response

```
{
  "error": "Batch not found with ID: 123"
}
```

---

## 📈 Future Enhancements

* Add Student module with batch relationships
* Add Spring Security for authentication & authorization
* Add Frontend UI (React / Angular)
* Implement report generation (CSV, Excel)

---

## 👨‍💻 Author

**Tejas Sutar**

---

## ⭐ Conclusion

EduTrack is a simple and efficient backend system demonstrating how **Spring Boot + MongoDB** can be used to build scalable classroom management solutions.

