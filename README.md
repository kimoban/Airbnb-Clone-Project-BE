# Airbnb Clone Project

## Project Overview
The Airbnb Clone Project backend is built to simulate a real-world booking platform. It focuses on user management, property listings, bookings, payments, and reviews. This project is designed using modern backend technologies with a focus on scalability, security, and API-first development.

## Team Roles
### Backend Developer	
Build RESTful and GraphQL APIs, implement business logic, and handle authentication/authorization.
### Database Administrator	
Design, manage, and optimize the PostgreSQL database schema and indexing strategies.
### DevOps Engineer	
Set up Docker containers, CI/CD pipelines, and ensure smooth deployments.
Facilitates cooperation between development and operations teams
Builds continuous integration and continuous delivery (CI/CD) pipelines for faster delivery
### QA Engineer
Test endpoints, automate test cases, and ensure system reliability.
Makes sure an application performs according to requirements
Spots functional and non-functional defects

## Technology Stack
Django:	Web framework for building RESTful APIs.
Django REST Framework (DRF):	Simplifies API creation and management.
GraphQL:	Provides flexible and efficient data querying.
PostgreSQL	Relational database used for storing structured data.
Celery:	Handles background tasks like sending emails or payment processing.
Redis:	Caching and session management to boost performance.
Docker:	Ensures consistent development environments across systems.
GitHub Actions:	Automates tests and deployments (CI/CD).

## Database Design
### User Authentication
Endpoints: /users/, /users/{user_id}/
Features: Register new users, authenticate, and manage user profiles.

### Property Management
Endpoints: /properties/, /properties/{property_id}/
Features: Create, update, retrieve, and delete property listings.

### Booking System
Endpoints: /bookings/, /bookings/{booking_id}/
Features: Make, update, and manage bookings, including check-in and check-out details.

### Payment Processing
Endpoints: /payments/
Features: Handle payment transactions related to bookings.

### Review System
Endpoints: /reviews/, /reviews/{review_id}/
Features: Post and manage reviews for properties.

## Feature Breakdown
User Management: Allows users to register, log in, and manage profiles securely.
Property Management: Hosts can list, update, and delete their rental properties.
Booking System: Enables guests to reserve properties with check-in/out details.
Payment Processing: Securely handles booking payments and logs transaction details.
Review System: Users can leave reviews and rate their stays.
Optimized Performance: Indexing and caching boost speed and reduce server load.

## API Security
Key Security Measures:
Authentication: Token-based (JWT) login for users.

Authorization: Ensures users only access their resources (e.g., bookings).

Rate Limiting: Prevents brute-force and abuse of endpoints.

Input Validation: Protects against SQL injection and XSS.

Secure Payments: Sensitive data is handled securely via HTTPS and payment gateway encryption.

## Importance

Protects user data and personal information.

Prevents unauthorized access and tampering.

Ensures financial transactions are secure.

## CI/CD Pipeline
What is CI/CD?
CI/CD (Continuous Integration / Continuous Deployment) automates testing and deployment of code, improving reliability and development speed.
### Tools Used
GitHub Actions: Automates tests on pull requests and pushes.
Docker: Ensures the app runs in consistent environments across dev and prod.
Docker Compose: For managing multi-container services like Django, Redis, and PostgreSQL.
