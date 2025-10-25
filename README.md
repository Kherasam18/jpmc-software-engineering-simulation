# 🏦 JP Morgan Chase – Software Engineering Job Simulation (Midas Core)

This repository contains my implementation of the **JP Morgan Chase Software Engineering Virtual Internship** hosted on [Forage](https://www.theforage.com/).

The project simulates working on **Midas Core**, a backend microservice designed to process financial transactions securely and efficiently.

---

## 🚀 Overview

During this virtual internship, I completed **five real-world inspired engineering tasks** covering key backend development concepts:

- ⚙️ **Apache Kafka** – Event stream processing  
- 🧠 **Spring Boot** – Backend microservice development  
- 💾 **H2 Database** – In-memory data storage  
- 🧩 **JPA** – ORM and persistence  
- 🌐 **REST API** – External service integration  

Each task builds upon the previous one to form a complete, production-like financial transaction system based on **event-driven architecture**.

---

## 📂 Project Structure

| Task | Area | Description |
|------|------|-------------|
| **Task 1** | Project Setup | Initialized Spring Boot project and Maven dependencies |
| **Task 2** | Kafka Integration | Consumed transaction messages via Kafka topics |
| **Task 3** | H2 Integration | Validated and persisted transactions in-memory |
| **Task 4** | Incentive API | Integrated external API for incentive calculation |
| **Task 5** | REST Controller | Exposed balance query endpoint `/balance` |

---

## ✅ Task Details

### 🧩 Task 1: Project Setup & Dependencies
**Objective:**  
Initialize the base **Spring Boot** project using **Java 17** and configure required dependencies.

**Dependencies Used:**
| Dependency | Version |
|-------------|----------|
| spring-boot-starter-data-jpa | 3.2.5 |
| spring-boot-starter-web | 3.2.5 |
| spring-kafka | 3.1.4 |
| h2 | 2.2.224 |
| spring-boot-starter-test | 3.2.5 |
| spring-kafka-test | 3.1.4 |
| testcontainers-kafka | 1.19.1 |

**What I Did:**
- Forked and cloned the starter repo  
- Configured dependencies in `pom.xml`  
- Verified initial tests successfully  
✅ *Passed `TaskOneTests`*

---

### 📦 Task 2: Kafka Integration
**Objective:**  
Implement a **Kafka listener** to read and process incoming transaction messages.

**What I Did:**
- Configured Kafka consumer with Spring Boot  
- Implemented `@KafkaListener` for message consumption  
- Validated JSON deserialization via embedded Kafka broker  
✅ *Passed `TaskTwoTests`*

---

### 💾 Task 3: H2 Database Integration & Transaction Validation
**Objective:**  
Validate and store financial transactions using **JPA** with an **H2 database**.

**Validation Rules:**
- Sender and recipient must exist  
- Sender must have sufficient balance  
- Invalid transactions are discarded  

**What I Did:**
- Created `TransactionRecord` entity  
- Implemented validation logic and balance updates  
- Integrated JPA repositories for persistence  
✅ *Passed `TaskThreeTests`*

---

### 🤝 Task 4: Incentive API Integration
**Objective:**  
Send valid transactions to an **Incentive API**, receive bonus amounts, and apply them to recipient balances.

**What I Did:**
- Used `RestTemplate` for POST requests  
- Consumed API from `http://localhost:8080/incentive`  
- Updated balance logic to include incentives  
✅ *Passed `TaskFourTests`*

---

### 🌐 Task 5: Expose Balance Query API
**Objective:**  
Develop a REST endpoint `/balance` that:
- Accepts `userId` as a parameter  
- Returns the user’s current balance (JSON)  
- Defaults to 0 if user does not exist  

**What I Did:**
- Created REST controller on port `33400`  
- Fetched user data via JPA  
- Returned response in `Balance` class format  
✅ *Passed `TaskFiveTests`*

---

## 🧠 Tech Stack

| Category | Technology |
|-----------|-------------|
| Language | Java 17 |
| Framework | Spring Boot |
| Messaging | Apache Kafka (Embedded) |
| Database | H2 (In-Memory) |
| ORM | JPA |
| Build Tool | Maven |
| Testing | Testcontainers, Spring Boot Test |
| IDE | IntelliJ IDEA |
| API Client | RestTemplate |

---

## 💡 Key Learnings

- Built a production-style Spring Boot microservice  
- Implemented **event-driven communication** with Kafka  
- Integrated external **REST APIs** within microservices  
- Tested using **embedded Kafka** and **H2 databases**  
- Designed robust **transaction validation and persistence logic**

---

## 🏁 Certification

**Certification:** [Software Engineering Job Simulation – JP Morgan Chase (Forage)]([https://www.theforage.com/](https://drive.google.com/file/d/1v9EU2Z4o9VtvTpMtyJzu2UbZREz_yU_a/view?usp=sharing))  
**Completed Tasks:**  
✔ Project Setup  
✔ Kafka Integration  
✔ H2 Integration  
✔ REST API Integration  
✔ REST Controller Development  

---

## 🔗 Connect With Me

📧 **Email:** [kherasam18@gmail.com](mailto:kherasam18@gmail.com)  
💼 **LinkedIn:** [linkedin.com/in/samkhera](https://www.linkedin.com/in/sam-khera-744811203/)  
🧠 **Blog:** [medium.com/@kherasam18](https://medium.com/@kherasam18)

---

⭐ **Pro Tip:**  
Include a **certificate PDF or image** in your repository and link it in the README for credibility.

