# Online Fitness Tracking Application

**Online Fitness Tracking Application** is a web-based fitness platform where users can access various resources to support their fitness journey, including blogs, live tracking, and personal progress insights. An admin panel provides control over content and user management.

---

## Table of Contents
- [Features](#features)
- [Database Schema](#database-schema)
- [Technologies Used](#technologies-used)

---

## Features
- **User Registration & Profile Management**: Allows users to sign up, manage their profile, and track fitness progress.
- **Fitness Tracking**: Users can log sessions with details like calories burned, steps, and heart rate.
- **Blogs & Community Engagement**: Users and admins can post fitness-related blogs, and users can engage by adding comments.
- **Admin Panel**: Administrators have access to manage users, blogs, and review logs of actions taken on the platform.
- **Notifications**: Notifications for users regarding updates, reminders, or goals.

---

# Database Schema

This project uses a relational database with the following main tables:

### Users
Stores user information, including profile data.

| Field        | Type          | Description                       |
|--------------|---------------|-----------------------------------|
| id           | INT (Primary) | Unique identifier for the user    |
| username     | STRING        | Display name for the user         |
| email        | STRING        | User's email address              |
| password     | STRING        | Hashed password                   |
| createdAt    | TIMESTAMP     | Account creation timestamp        |
| updatedAt    | TIMESTAMP     | Last profile update timestamp     |

### User_Fitness_Profile
Stores details specific to each user's fitness goals and profile.

| Field        | Type          | Description                       |
|--------------|---------------|-----------------------------------|
| id           | INT (Primary) | Unique identifier                 |
| userId       | INT (Foreign) | Reference to the user             |
| weight       | FLOAT         | User's weight in kilograms        |
| height       | FLOAT         | User's height in centimeters      |
| fitnessGoals | TEXT          | Fitness goals description         |
| createdAt    | TIMESTAMP     | Profile creation timestamp        |

### Tracking_Sessions
Records each user's fitness activities and tracking sessions.

| Field        | Type          | Description                       |
|--------------|---------------|-----------------------------------|
| id           | INT (Primary) | Unique identifier                 |
| userId       | INT (Foreign) | Reference to the user             |
| activityType | STRING        | Type of activity (e.g., running)  |
| duration     | INT           | Duration in minutes               |
| calories     | INT           | Calories burned                   |
| steps        | INT           | Steps taken during the session    |
| date         | DATE          | Session date                      |

### Blogs
Contains blog posts created by users and admins.

| Field        | Type          | Description                       |
|--------------|---------------|-----------------------------------|
| id           | INT (Primary) | Unique identifier for the blog    |
| title        | STRING        | Blog title                        |
| content      | TEXT          | Blog content                      |
| authorId     | INT (Foreign) | Reference to the author           |
| createdAt    | TIMESTAMP     | Blog creation timestamp           |
| updatedAt    | TIMESTAMP     | Last blog update timestamp        |

### Comments
Stores comments on blog posts.

| Field        | Type          | Description                       |
|--------------|---------------|-----------------------------------|
| id           | INT (Primary) | Unique identifier                 |
| blogId       | INT (Foreign) | Reference to the blog             |
| userId       | INT (Foreign) | Reference to the commenter        |
| comment      | TEXT          | Comment content                   |
| createdAt    | TIMESTAMP     | Comment creation timestamp        |

### Admin_Panel
Defines admin access with specific permissions.

| Field        | Type          | Description                       |
|--------------|---------------|-----------------------------------|
| id           | INT (Primary) | Unique identifier                 |
| adminName    | STRING        | Admin username                    |
| email        | STRING        | Admin email address               |
| role         | STRING        | Role (e.g., SuperAdmin, Moderator)|
| createdAt    | TIMESTAMP     | Admin account creation timestamp  |

### Logs
Tracks actions taken by admins and other critical events.

| Field        | Type          | Description                       |
|--------------|---------------|-----------------------------------|
| id           | INT (Primary) | Unique identifier                 |
| adminId      | INT (Foreign) | Reference to the admin            |
| action       | STRING        | Description of the action         |
| timestamp    | TIMESTAMP     | Timestamp of the action           |

### Notifications
Manages notifications sent to users.

| Field        | Type          | Description                       |
|--------------|---------------|-----------------------------------|
| id           | INT (Primary) | Unique identifier                 |
| userId       | INT (Foreign) | Reference to the user             |
| type         | STRING        | Notification type (e.g., reminder)|
| message      | TEXT          | Notification content              |
| isRead       | BOOLEAN       | Read status of the notification   |
| createdAt    | TIMESTAMP     | Notification creation timestamp   |

---

# Technologies Used

### Frontend
- **HTML**
- **CSS**
- **JavaScript**

### Backend
- **Node.js**
- **Express.js**

### Database
- **MySQL** (or any relational database of choice)

### Authentication
- **JWT** (JSON Web Tokens)

### Environment Management
- **dotenv**


<h2>Preview 1</h2>
<img src="https://github.com/user-attachments/assets/b70e1f1c-256c-4ea9-9628-ed1c96d1d8c1"><br><br>
<h2>Preview 2</h2>
<img src="https://github.com/user-attachments/assets/a62df609-73f5-469b-b9c7-a2bfd570c07c"><br><br>
<h2>Preview 3</h2>
<img src="https://github.com/user-attachments/assets/ecc6ee8d-4da0-48c7-8600-312c34c1b473">
