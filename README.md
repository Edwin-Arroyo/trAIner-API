# trAIner-API

AI-Powered Fitness App Backend API

## Overview

trAIner-API is the backend service for an AI-powered fitness application that provides personalized workout plans, meal plans, and fitness regimens tailored to individual user needs. The application leverages OpenAI's API to generate custom fitness recommendations based on user goals, preferences, and constraints.

## Features

- **Custom Workout Plans**: AI-generated workout routines based on user fitness level, goals, and available equipment
- **Personalized Meal Plans**: Tailored nutrition recommendations considering dietary preferences, restrictions, and fitness objectives
- **Fitness Regimens**: Comprehensive training programs that adapt to user progress and preferences
- **User Management**: Secure authentication and user profile management
- **Progress Tracking**: Monitor fitness progress and adjust recommendations accordingly
- **AI Integration**: OpenAI API integration for intelligent fitness and nutrition recommendations

## Technology Stack

- **Framework**: Spring Boot 3.2.0
- **Language**: Java 17
- **Database**: MySQL
- **Security**: Spring Security
- **AI Integration**: OpenAI API
- **Build Tool**: Maven
- **API Documentation**: Spring Boot Actuator

## Getting Started

### Prerequisites

- Java 17 or higher
- Maven 3.6+
- MySQL 8.0+
- OpenAI API Key

### Installation

1. Clone the repository:

```bash
git clone <repository-url>
cd trAIner-API
```

2. Configure the database:

   - Create a MySQL database named `trainer_db`
   - Update database credentials in `src/main/resources/application.properties`

3. Set up OpenAI API:

   - Obtain an API key from OpenAI
   - Configure the API key in your environment variables

4. Run the application:

```bash
mvn spring-boot:run
```

The API will be available at `http://localhost:8080/api`

### API Endpoints

- **Health Check**: `GET /api/health`
- **Actuator**: `GET /api/actuator/health`

## Configuration

Key configuration properties in `application.properties`:

- Server port: 8080
- Database: MySQL (trainer_db)
- CORS: Enabled for frontend integration
- Security: Basic authentication setup

## Development

The project follows standard Spring Boot conventions with the following package structure:

- `com.trainer.controller` - REST API controllers
- `com.trainer.config` - Configuration classes
- `com.trainer.service` - Business logic services
- `com.trainer.repository` - Data access layer
- `com.trainer.model` - Entity models

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.
