
# Uber FullStack

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Folder Structure](#folder-structure)



## Project Overview
Uber FullStack is a web application that mimics the functionality of the Uber platform, allowing users to book rides. This project is designed to demonstrate full-stack development skills, including both frontend and backend technologies.

## Features
- User authentication and authorization
- Ride booking
- Real-time tracking of rides
- User and driver profiles

## Technologies Used
- **Frontend:**
  - React
  - Tailwind CSS
  - Vite
  - JavaScript

- **Backend:**
  - Node.js
  - Express.js
  - MongoDB
  - Mongoose

- **Others:**
  - Git for version control
  - Postman for API testing

## Installation
To set up the project locally, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Mousam861/Uber_FullStack.git
   cd Uber_FullStack
   ```

2. **Install backend dependencies:**
   Navigate to the backend directory and install the required packages.
   ```bash
   cd Backend
   npm install
   ```

3. **Set up the database:**
   Ensure you have MongoDB installed and running. Create a new database for the project.

4. **Configure environment variables:**
   Create a `.env` file in the Backend directory and add the necessary environment variables (e.g., database connection string, JWT secret).

5. **Run the backend server:**
   ```bash
   npm start
   ```

6. **Install frontend dependencies:**
   Navigate to the frontend directory and install the required packages.
   ```bash
   cd ../frontend
   npm install
   ```

7. **Run the frontend server:**
   ```bash
   npm run dev
   ```

8. **Access the application:**
   Open your browser and go to `http://localhost:3000` to view the application.

## Usage
- **User  Registration:** Users can register by providing their details.
- **Login:** Users can log in to their accounts to book rides.
- **Booking a Ride:** Users can select their pickup and drop-off locations to book a ride.
- **Driver Interaction:** Drivers can accept ride requests and manage their profiles.

## Folder Structure
```plaintext
Uber_FullStack/
├── Backend/
│   ├── controllers/
│   ├── middlewares/
│   ├── models/
│   ├── routes/
│   ├── db/
│   ├── app.js
│   └── package.json
└── frontend/
    ├── src/
    │   ├── components/
    │   ├── pages/
    │   ├── context/
    │   ├── assets/
    │   ├── App.jsx
    │   └── index.jsx
    ├── public/
    ├── package.json
    └── vite.config.js
```


Developed by Mousam44. Feel free to reach out at mousambarui@gmail.com for any questions or suggestions.