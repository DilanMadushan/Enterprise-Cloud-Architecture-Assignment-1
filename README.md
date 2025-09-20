# Course Service (Spring Boot + GCP MySQL) 🌐🐬☕️

This project is a **Spring Boot application** that manages course data and connects to a **MySQL database** hosted on *Google Cloud SQL*.  
It follows best practices for cloud-ready development by using **Spring Profiles** to separate configurations for local and cloud environments.

With this setup, you can easily switch between development and production, ensuring smooth database connectivity and environment management.

---

## 👤 Personal Details

- **Name**: Dilan Madushanka Fernando
- **Batch**: Panadura
- **Student ID**: 2301671122

---

## 🎬 Video Demonstration on GCP
[Watch the demo](https://drive.google.com/file/d/1oCF_GGqyHeFlysvPfsBsTMvMmDnfDTaH/view?usp=sharing)

---

## 🔧 Prerequisites
Before running the project, make sure you have the following installed and configured:

- ☕ **Java 21 LTS**
- 🐬 **MySQL** (local or Google Cloud SQL)
- ☁️ **Google Cloud SQL (MySQL) Instance**

---

## 🗄 Database Setup

### ☁️ Cloud Configuration (`application-gcp.properties`)

Replace the placeholders with your own database credentials:

```properties
spring.datasource.url=jdbc:mysql://<PUBLIC_GCP_IP>:3306/<DB_NAME>?createDatabaseIfNotExist=true&useSSL=false&allowPublicKeyRetrieval=true
spring.datasource.username=<GCP_MYSQL_USERNAME>
spring.datasource.password=<GCP_MYSQL_PASSWORD>
