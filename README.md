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

### Spring Boot OAuth2 Client
- **Path**: `spring-boot-outh2-client/`
- **Description**: OAuth2 client implementation for third-party authentication
- **Features**: OAuth2 client credentials, token management, secure API access

### Spring Boot OAuth2 Server
- **Path**: `spring-boot-outh2-server/`
- **Description**: OAuth2 authorization server implementation
- **Features**: OAuth2 authorization server, token endpoints, client registration

### Spring Security Facebook Login
- **Path**: `springsecurity-facebook-login/`
- **Description**: Facebook social login integration
- **Features**: Facebook OAuth2 integration, social authentication, user profile mapping

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

# Run Spring Boot OAuth2 Client
cd spring-boot-outh2-client
mvn spring-boot:run

# Run Spring Boot OAuth2 Server
cd spring-boot-outh2-server
mvn spring-boot:run

# Run Spring Security Facebook Login
cd springsecurity-facebook-login
mvn spring-boot:run
```

### Service Endpoints

Once applications are running, you can access:

- **Spring Security App**: http://localhost:8080
- **Spring Security LDAP App**: http://localhost:8081
- **Spring Boot OAuth2 Client**: http://localhost:8082
- **Spring Boot OAuth2 Server**: http://localhost:8083
- **Spring Security Facebook Login**: http://localhost:8084

## Development

### Project Structure

```
spring-security/
├── pom.xml                           # Parent POM with common configuration
├── README.md                         # This file
├── spring-security-app/              # Basic security implementation
├── spring-security-ldap-app/         # LDAP security implementation
├── spring-boot-outh2-client/         # OAuth2 client implementation
├── spring-boot-outh2-server/         # OAuth2 server implementation
└── springsecurity-facebook-login/    # Facebook login integration
```

### Configuration

Each module contains its own application configuration:
- Security configurations in respective Security classes
- Application properties in `application.properties`
- User credentials and role definitions

