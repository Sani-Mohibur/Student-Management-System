# Student Management System

A web application for managing student records, built with Java, Spring Boot, Spring Data JPA, and Thymeleaf. This project implements complete CRUD (Create, Read, Update, Delete) functionality.

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-C71A36?style=for-the-badge&logo=apache-maven&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Thymeleaf](https://img.shields.io/badge/Thymeleaf-005F0F?style=for-the-badge&logo=thymeleaf&logoColor=white)

## ✨ Features

* **View All Students:** A paginated list displaying all students in the database.
* **Add New Student:** A form to create and save a new student record.
* **Update Student Information:** Edit the details of any existing student.
* **Delete Student:** Remove a student record from the system.
* **Server-Side Rendering:** A dynamic user interface rendered on the server using Thymeleaf.
* **Responsive UI:** The frontend is built with Bootstrap, making it compatible with different screen sizes.

## 🛠️ Technologies & Tools Used

* **Backend:** Java, Spring Boot, Spring MVC, Spring Data JPA
* **Frontend:** Thymeleaf, HTML, Bootstrap CSS
* **Database:** MySQL
* **Build Tool:** Maven

## 🚀 Getting Started

To get a local copy up and running, follow these steps.

### Prerequisites

* **JDK 17** or later
* **Apache Maven**
* **MySQL Server**

### Installation & Setup

1.  **Clone the repository:**
    ```sh
    git clone [https://github.com/Sani-Mohibur/Student-Management-System.git](https://github.com/Sani-Mohibur/Student-Management-System.git)
    cd Student-Management-System
    ```

2.  **Create MySQL Database:**
    Open your MySQL client and create a new database for the project.
    ```sql
    CREATE DATABASE sms_db;
    ```

3.  **Configure Database Connection:**
    Open the `src/main/resources/application.properties` file. Update the `spring.datasource.url`, `spring.datasource.username`, and `spring.datasource.password` properties to match your local MySQL setup.

    ```properties
    spring.datasource.url=jdbc:mysql://localhost:3306/sms_db?useSSL=false
    spring.datasource.username=your_mysql_username
    spring.datasource.password=your_mysql_password
    spring.jpa.hibernate.ddl-auto=update
    spring.jpa.show-sql=true
    ```

4.  **Build the project using Maven:**
    This will download all the required dependencies.
    ```sh
    mvn clean install
    ```

5.  **Run the application:**
    ```sh
    mvn spring-boot:run
    ```
    The application will start on the default port `8080`.

6.  **Access the Application:**
    Open your web browser and go to `http://localhost:8080/students`.
