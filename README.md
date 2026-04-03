# Spring Security Projects

A comprehensive collection of Spring Security demonstration projects showcasing various authentication and authorization mechanisms.

## Overview

This parent project manages multiple Spring Security applications, each demonstrating different security concepts and implementations.

## Modules

### Spring Security App
- **Path**: `spring-security-app/`
- **Description**: Basic Spring Security implementation with form-based authentication
- **Features**: User authentication, role-based authorization, secure endpoints

### Spring Security LDAP App
- **Path**: `spring-security-ldap-app/`
- **Description**: LDAP-based authentication integration
- **Features**: LDAP directory authentication, enterprise security integration

## Technology Stack

- **Java 8**
- **Spring Boot 1.5.2.RELEASE**
- **Spring Security**
- **Maven** - Build tool and dependency management
- **LDAP** - Directory service authentication (LDAP module)

## Quick Start

### Prerequisites
- Java 8 or higher
- Maven 3.3 or higher

### Building the Project

```bash
# Build all modules
mvn clean install

# Build specific module
mvn clean install -pl spring-security-app

# Skip tests during build
mvn clean install -DskipTests
```

### Running Applications

```bash
# Run Spring Security App
cd spring-security-app
mvn spring-boot:run

# Run Spring Security LDAP App
cd spring-security-ldap-app
mvn spring-boot:run
```

### Service Endpoints

Once applications are running, you can access:

- **Spring Security App**: http://localhost:8080
- **Spring Security LDAP App**: http://localhost:8081

## Development

### Project Structure

```
spring-security/
├── pom.xml                           # Parent POM with common configuration
├── README.md                         # This file
├── spring-security-app/              # Basic security implementation
└── spring-security-ldap-app/         # LDAP security implementation
```

### Configuration

Each module contains its own application configuration:
- Security configurations in respective Security classes
- Application properties in `application.properties`
- User credentials and role definitions

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests for new functionality
5. Run the test suite
6. Submit a pull request

## License

This project is for educational and demonstration purposes.
