# Cleaning Company Website - Project Proposal
1. Tech Stack
Frontend: React (with Tailwind CSS or Material-UI for styling(suggested by mentor))
Backend: Node.js with Express.js
Database: MongoDB (hosted on MongoDB Atlas)
Authentication: JSON Web Tokens (JWT)
Hosting: Vercel/Netlify for frontend, Render/Heroku for backend
2. Focus of the Project
This will be an evenly focused full-stack application, ensuring both frontend and backend functionalities work seamlessly together.
3. Type of Application
This project will be a web-based application that allows users to book cleaning services easily.
4. Project Goal
The goal of this project is to create a simple and efficient booking system for a cleaning company where customers can:
View available cleaning services
Schedule a cleaning appointment
Manage their bookings
Admins can view and manage bookings
5. Target Users
Customers: Individuals or businesses looking for cleaning services.
Admin: The cleaning company management team who will oversee bookings and service offerings.
6. Data Plan
The application will store and manage the following types of data:
User Data: Name, email, password (hashed), and role (customer/admin).
Service Data: Service names, descriptions, and prices.
Booking Data: User ID, service ID, date, time, and status (pending, completed, or canceled).
Data Source & Collection
The data will be managed in a custom-built API using MongoDB.
No external APIs are required at this stage.
7. Database Schema (MongoDB)
Users Collection (users)
{
  "_id": "ObjectId",
  "name": "John Doe",
  "email": "john@example.com",
  "password": "hashed_password",
  "role": "customer" // or "admin"
}

Services Collection (services)
{
  "_id": "ObjectId",
  "name": "Deep Cleaning",
  "description": "Thorough cleaning of all surfaces, carpets, and appliances.",
  "price": 100
}

Bookings Collection (bookings)
{
  "_id": "ObjectId",
  "userId": "ObjectId",
  "serviceId": "ObjectId",
  "date": "2025-03-01",
  "time": "10:00 AM",
  "status": "pending" // or "completed", "canceled"
}

8. Project Approach
Challenges & Considerations
Ensuring secure authentication and authorization.
Managing bookings effectively (handling overlapping schedules, cancellations, etc.).
Creating a responsive and user-friendly UI.
User Flow
Customers visit the website and browse available cleaning services.
They sign up/log in to schedule a cleaning appointment.
They select a service, date, and time for booking.
Admins can log in to view, manage, and update bookings.
9. Stretch Goals
(These are not mandatory for completion but can be added later as enhancements.)
Integrate payment processing (Stripe/PayPal)
Add a customer dashboard for managing past bookings
Implement a notification system (email reminders for upcoming bookings)

