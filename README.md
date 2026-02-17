# Secure REST API

Production-ready secure REST API built with Spring Boot, Oracle and JWT authentication.

---

## 🚀 Tech Stack

- Java 17
- Spring Boot 3
- Spring Data JPA (Hibernate)
- Oracle Database
- Maven
- Lombok
- Jakarta Validation

---

## 📂 Packages

- `config` – application & security configuration
- `controller` – REST endpoints
- `service` – business logic
- `repository` – database access (JPA)
- `domain` – entities / domain models
- `dto` – request/response DTOs
- `exception` – custom exceptions + global error handling

---

## ⚙️ Configuration

Example `src/main/resources/application.yaml`:

```yaml
spring:
  datasource:
    url: jdbc:oracle:thin:@//localhost:1521/orclpdb
    username: HR
    password: YOUR_PASSWORD
    driver-class-name: oracle.jdbc.OracleDriver

  jpa:
    hibernate:
      ddl-auto: none
    properties:
      hibernate:
        dialect: org.hibernate.dialect.OracleDialect
    show-sql: true

server:
  port: 8080
