# Online Fitness Tracking Application

**Online Fitness Tracking Application** is a web-based fitness platform where users can access various resources to support their fitness journey, including blogs, live tracking, and personal progress insights. An admin panel provides control over content and user management.

---

## Table of Contents
- [Features](#features)
- [Architecture Overview](#architecture-overview)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Project Structure](#project-structure)
-  [Outcome](#outcome)

---

## Features

- **User Registration & Profile Management**: Users can sign up, manage profiles, and track fitness progress.
- **Fitness Tracking**: Log fitness sessions with details like calories burned, steps taken, and heart rate.
- **Blogs & Community Engagement**: Users and admins can post fitness blogs, and users can interact by commenting.
- **Admin Panel**: Admins have the ability to manage users, blogs, and review platform activity logs.
- **Notifications**: Users receive notifications for updates, reminders, and goal tracking.

---
## Architecture Overview

![Fitness Diagram](https://example.com/fitness-architecture.jpg)

### Backend Architecture
The backend is designed for scalability and flexibility, implemented using **Node.js** and **Express.js**. Key components include:

- **Node.js Server**: A server built on **Node.js** providing a scalable environment for handling multiple user requests.
- **RESTful API**: The platform uses REST APIs to exchange data, returning JSON responses.
- **Authentication**: **JWT (JSON Web Tokens)** are used for secure user authentication and session management.
- **Relational Database**: The application stores data using a relational database, with **MySQL** as the primary choice.

### Frontend Architecture
The frontend ensures a user-friendly experience, incorporating:

- **HTML/CSS/JavaScript**: Basic technologies for building responsive and dynamic webpages.
- **Frontend Frameworks**: Bootstrap is used to provide a responsive and clean design, ensuring mobile-friendliness.
- **User Interaction**: JavaScript is used for handling dynamic interactions, such as form submissions and user notifications.
  
## Technologies Used

### Backend Technologies
- **Node.js**  
- **Express.js**  
- **MySQL** (or any relational database)  
- **JWT (JSON Web Tokens)** for authentication

### Frontend Technologies
- **HTML/CSS/JavaScript**  
- **Bootstrap**  

### Environment Management
- **dotenv** for managing environment variables

### Development Tools
- **Git**  
- **GitHub**  
- **Visual Studio Code**

  ## Installation

To set up the project locally:

### Clone the Repository
```bash
# Start: Clone repository
git clone https://github.com/user-attachments/Online-Fitness-Tracking-App
cd Online-Fitness-Tracking-App
# End: Clone repository
```

## Project Structure

```plaintext
FitnessTracker/
├── src/
│   ├── controllers/               # Controller files handling requests
│   ├── models/                    # Models representing database entities
│   ├── routes/                    # API routes for fitness tracking and user management
│   ├── services/                  # Services for business logic
│   ├── views/                     # HTML views for user and admin interfaces
│   ├── config/                    # Configuration files (e.g., database, JWT secrets)
│   └── database/                  # Database setup and schema
├── public/                        # Static assets (CSS, JS, images)
│   ├── css/                       # CSS files
│   ├── js/                        # JavaScript files
│   └── images/                    # Image assets
├── .env                           # Environment variables for configuration
├── server.js                      # Entry point for the application
└── README.md                      # Project documentation
```

## Outcome
<h2>Preview 1</h2>
<img src="https://github.com/user-attachments/assets/b70e1f1c-256c-4ea9-9628-ed1c96d1d8c1"><br><br>
<h2>Preview 2</h2>
<img src="https://github.com/user-attachments/assets/a62df609-73f5-469b-b9c7-a2bfd570c07c"><br><br>
<h2>Preview 3</h2>
<img src="https://github.com/user-attachments/assets/ecc6ee8d-4da0-48c7-8600-312c34c1b473">
