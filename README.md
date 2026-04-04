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

### Spring Security Facebook Login
- **Path**: `springsecurity-facebook-login/`
- **Description**: Facebook OAuth2 login integration
- **Features**: Social authentication, OAuth2 client configuration, user profile retrieval

### Spring Boot OAuth2 Client
- **Path**: `spring-boot-outh2-client/`
- **Description**: OAuth2 client implementation for accessing protected resources
- **Features**: Multiple OAuth2 providers, token management, authorization code flow

### Spring Boot OAuth2 Authorization Server
- **Path**: `spring-boot-outh2-server/`
- **Description**: Complete OAuth2 Authorization Server implementation
- **Features**: JWT token issuance, client management, token introspection

## Technology Stack

- **Java 8+**
- **Spring Boot 2.x**
- **Spring Security**
- **Spring Security OAuth2**
- **Maven** - Build tool and dependency management
- **LDAP** - Directory service authentication (LDAP module)
- **OAuth2** - OAuth2 client and server implementations
- **JWT** - JSON Web Token support

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

# Run Spring Security Facebook Login
cd springsecurity-facebook-login
mvn spring-boot:run

# Run OAuth2 Client
cd spring-boot-outh2-client
mvn spring-boot:run

# Run OAuth2 Authorization Server
cd spring-boot-outh2-server
mvn spring-boot:run
```

### Service Endpoints

Once applications are running, you can access:

- **Spring Security App**: http://localhost:8080
- **Spring Security LDAP App**: http://localhost:8081
- **Spring Security Facebook Login**: http://localhost:8082
- **OAuth2 Client**: http://localhost:8083
- **OAuth2 Authorization Server**: http://localhost:9000

## Development

### Project Structure

```
spring-security/
├── pom.xml                           # Parent POM with common configuration
├── README.md                         # This file
├── .gitmodules                       # Git submodules configuration
├── spring-security-app/              # Basic security implementation
├── spring-security-ldap-app/         # LDAP security implementation
├── springsecurity-facebook-login/    # Facebook OAuth2 login
├── spring-boot-outh2-client/         # OAuth2 client implementation
└── spring-boot-outh2-server/         # OAuth2 authorization server
```

### Configuration

Each module contains its own application configuration:
- Security configurations in respective Security classes
- Application properties in `application.properties`
- User credentials and role definitions
- OAuth2 provider configurations (for OAuth2 modules)

### Git Submodules

This project uses Git submodules to manage individual Spring Security projects. To work with submodules:

```bash
# Initialize and update all submodules
git submodule update --init --recursive

# Update a specific submodule
git submodule update --remote springsecurity-facebook-login

# Pull latest changes for all submodules
git submodule foreach git pull origin main
```

