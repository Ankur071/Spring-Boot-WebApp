# Simple Web App

A Spring Boot web application demo project.

## Prerequisites

- Java 17
- Maven 3.x

## Configuration

This application uses environment variables for sensitive configuration like database credentials. This ensures credentials are never stored in version control.

### Setting Up Environment Variables

1. Copy the `.env.example` file to `.env`:
   ```bash
   cp .env.example .env
   ```

2. Edit `.env` and fill in your actual credentials:
   ```
   DB_USERNAME=your_actual_username
   DB_PASSWORD=your_actual_password
   ```

3. Load the environment variables before running the application:
   ```bash
   source .env
   export DB_USERNAME
   export DB_PASSWORD
   ```

Alternatively, you can set environment variables directly in your IDE or system.

## Running the Application

```bash
./mvnw spring-boot:run
```

The application will start on port 8090.

## Building

```bash
./mvnw clean package
```

## Testing

```bash
./mvnw test
```
