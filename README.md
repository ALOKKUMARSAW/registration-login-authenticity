# **Registration and Login Authenticity**

## **Project Overview**

This project is a comprehensive user registration and login module built with **Spring Boot**, **Spring MVC**, **Spring Security**, and **Thymeleaf**. It provides a robust foundation for managing user authentication and authorization in web applications.

## **Key Features**

- **User Registration**: Allows new users to create accounts with unique usernames and secure passwords.
- **User Login**: Authenticates users based on their credentials, granting access to protected resources.
- **Password Encryption**: Utilizes **BCrypt** to securely hash user passwords.
- **Role-Based Authorization**: Implements role-based access control to manage user permissions.
- **Form Validation**: Ensures user inputs meet specified criteria during registration and login processes.

## **Tech Stack**

- **Backend**: Java, Spring Boot, Spring MVC, Spring Security
- **Frontend**: Thymeleaf
- **Database**: MySQL
- **Build Tool**: Maven

## **Getting Started**

### **Prerequisites**

- **Java Development Kit (JDK)** 17 or higher
- **Maven** 3.8.1 or higher
- **MySQL** 8.0 or higher

### **Installation Steps**

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/ALOKKUMARSAW/registration-login-authenticity.git
   cd registration-login-authenticity
   ```

2. **Configure the Database**:
   - Create a MySQL database named `user_db`.
   - Update the database configuration in `src/main/resources/application.properties`:
     ```properties
     spring.datasource.url=jdbc:mysql://localhost:3306/user_db
     spring.datasource.username=your_username
     spring.datasource.password=your_password
     ```

3. **Build and Run the Application**:
   - Use Maven to build the project:
     ```bash
     mvn clean install
     ```
   - Run the Spring Boot application:
     ```bash
     mvn spring-boot:run
     ```

4. **Access the Application**:
   - Navigate to `http://localhost:8080` in your web browser.

## **Project Structure**

```
src/
├── main/
│   ├── java/
│   │   └── com.example.registration/
│   │       ├── config/           # Spring Security Configurations
│   │       ├── controller/       # Controllers for handling web requests
│   │       ├── model/            # Entity models
│   │       ├── repository/       # Repository interfaces for data access
│   │       ├── service/          # Service layer for business logic
│   │       └── RegistrationApplication.java   # Main application class
│   └── resources/
│       ├── templates/            # Thymeleaf templates
│       ├── static/               # Static resources (CSS, JS)
│       └── application.properties  # Application configuration
└── pom.xml                       # Maven configuration file
```

## **License**

This project is licensed under the MIT License.
 




