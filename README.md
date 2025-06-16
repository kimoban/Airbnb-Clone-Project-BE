## Airbnb-Clone-Project-BE
Airbnb Clone Project
## Project Overview
The Airbnb Clone Project is a full-stack web application that replicates key features of Airbnb, focusing on backend development. It offers hands-on experience with building a scalable, secure, and feature-rich booking platform.

🎯 Goals:

Simulate a real-world software development environment

Implement backend architecture using Django

Integrate MySQL and GraphQL

Apply security best practices

Set up a CI/CD pipeline for automated deployment

## Team Roles
Backend Developer
Responsible for designing and implementing the application’s logic, APIs, and integrations. Focuses on handling data, authentication, and server-side operations.

Database Administrator
Designs and manages the MySQL database schema, ensures data consistency and integrity, and handles performance tuning.

DevOps Engineer
Implements CI/CD pipelines, manages Docker containers, and oversees the deployment process on cloud infrastructure.

Frontend Developer (optional)
Connects the backend APIs to the UI, focusing on a seamless user experience.

🧰 Technology Stack
Technology	Purpose
Django	Backend web framework for creating RESTful APIs
MySQL	Relational database for managing structured application data
GraphQL	Query language for flexible client-server data interaction
Docker	Containerization for consistent development and deployment
GitHub Actions	CI/CD automation tool for building, testing, and deploying code

🗃️ Database Design
Key Entities:
User

id, username, email, password

A user can book properties and post reviews.

Property

id, title, description, location, price

A property belongs to a user (host).

Booking

id, user_id, property_id, check_in, check_out

Represents a reservation made by a user.

Review

id, user_id, property_id, rating, comment

Reviews are tied to both users and properties.

Payment

id, booking_id, amount, payment_method, status

Records payment info linked to bookings.

Relationships:

One user can have many properties.

One property can have many bookings and reviews.

One booking leads to one payment.

🧩 Feature Breakdown
User Management: Users can sign up, log in, and manage their profiles securely.

Property Listings: Hosts can create, update, and delete property listings.

Booking System: Users can book available properties for specific dates.

Review System: Users can leave reviews and ratings for properties they’ve stayed in.

Payment Integration: Simulated payment system to handle booking payments.

🔐 API Security
Authentication: Uses JWT tokens to ensure only registered users can access protected endpoints.

Authorization: Restricts access to specific resources (e.g., only the host can modify their property).

Rate Limiting: Prevents API abuse by limiting requests per time interval.

Input Validation: Protects against SQL Injection and XSS by validating user input.

Why It’s Crucial:

User Protection: Prevents unauthorized access to personal data.

Transaction Safety: Secures payment-related endpoints.

Platform Integrity: Maintains trust and prevents misuse of the system.

🚀 CI/CD Pipeline
What is CI/CD?
Continuous Integration and Continuous Deployment (CI/CD) automate the development workflow, ensuring that code changes are automatically tested and deployed.

Tools:

GitHub Actions: Automates testing and deployment after code commits.

Docker: Ensures consistent environment across development, staging, and production.

Benefits:

Speeds up delivery

Reduces bugs in production

Improves collaboration among developers
