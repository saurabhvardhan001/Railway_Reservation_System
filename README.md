# Railway Reservation System

## Project Documentation

### Introduction
The Railway Reservation System is a comprehensive application designed to facilitate train ticket bookings, cancellations, and inquiries for users. This document provides an overview of the architecture, microservices, technology stack, features, and setup instructions for the system.

### Architecture
The Railway Reservation System is based on a microservices architecture, which allows for independence, scalability, and easier maintenance. The main components of the architecture include:

1. **User Service**: Handles user registrations, authentication, and profiles.
2. **Booking Service**: Manages all booking-related functionalities like reserving, modifying, and canceling tickets.
3. **Train Service**: Provides train schedules, availability, and details.
4. **Payment Service**: Facilitates payment processing for ticket bookings.
5. **Notification Service**: Sends notifications to users regarding booking confirmations, cancellations, etc.

### Microservices
Each microservice is designed to be a standalone application, communicating through REST APIs. This allows for flexibility in development and deployment, as well as the ability to use different databases and programming languages as needed.

### Technology Stack
- **Frontend**: React.js
- **Backend**: Node.js, Express.js
- **Database**: MongoDB for the user and booking services; MySQL for train schedules.
- **Message Broker**: RabbitMQ for service-to-service communication.
- **Containerization**: Docker for containerizing microservices.
- **Cloud Hosting**: AWS or any cloud provider for deployment.

### Features
- User Registration and Authentication
- Train Search and Availability Checks
- Ticket Booking and Cancellation
- Payment Integration (Credit/Debit Cards, UPI)
- User Notifications (Email/SMS)
- Admin Dashboard for train management and reporting

### Setup Instructions
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/saurabhvardhan001/Railway_Reservation_System.git
   cd Railway_Reservation_System
   ```
2. **Install Dependencies**:
   - For each microservice, navigate to its directory and run:
   ```bash
   npm install
   ```
3. **Set up the Environment Variables**:
   - Create a `.env` file in each microservice directory and configure the database and service URLs.
4. **Start the Services**:
   - Each microservice can be started using:
   ```bash
   npm start
   ```
   or using Docker:
   ```bash
   docker-compose up
   ```
5. **Access the Application**:
   - Open your browser and go to `http://localhost:<port>` for the respective service.

### Conclusion
The Railway Reservation System is designed to enhance user experience by providing a seamless booking process and robust service architecture. Follow the setup instructions to deploy the application locally.