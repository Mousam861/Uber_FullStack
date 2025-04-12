
# Frontend

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Folder Structure](#folder-structure)
- [Components](#components)
- [Context Providers](#context-providers)
- [Routing](#routing)
- [Styling](#styling)

## Overview
The frontend of the Uber FullStack project is built using React and Vite, providing a responsive and dynamic user interface for users to interact with the application. This section outlines how to set up and use the frontend application.

## Features
- User-friendly interface for booking rides
- Real-time updates for ride status
- Profile management for users and drivers
- Responsive design for mobile and desktop views
- Integration with backend services for data fetching

## Technologies Used
- **React**: A JavaScript library for building user interfaces.
- **Vite**: A fast build tool and development server for modern web projects.
- **Tailwind CSS**: A utility-first CSS framework for styling.
- **JavaScript**: The primary programming language used for development.

## Installation
To set up the frontend locally, follow these steps:

1. **Navigate to the frontend directory:**
   ```bash
   cd Uber_FullStack/frontend
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Start the development server:**
   ```bash
   npm run dev
   ```

4. **Open your browser:**
   - Go to `http://localhost:3000` to view the application.

## Usage
- **Home Page**: Users can view the home page to start booking rides.
- **Login/Signup**: Users can log in or create a new account.
- **Booking a Ride**: Users can enter their pickup and drop-off locations to book a ride.
- **Profile Management**: Users can manage their profiles and view ride history.

## Folder Structure```plaintext
frontend/
├── public/
│   ├── vite.svg
│   └── index.html
├── src/
│   ├── assets/
│   │   └── react.svg
│   ├── components/
│   │   ├── CaptainDetails.jsx
│   │   ├── ConfirmRide.jsx
│   │   ├── ConfirmRidePopUp.jsx
│   │   ├── FinishRide.jsx
│   │   ├── LiveTracking.jsx
│   │   ├── LocationSearchPanel.jsx
│   │   ├── LookingForDriver.jsx
│   │   ├── RidePopUp.jsx
│   │   ├── VehiclePanel.jsx
│   │   └── WaitingForDriver.jsx
│   ├── context/
│   │   ├── CaptainContext.jsx
│   │   ├── SocketContext.jsx
│   │   └── UserContext.jsx
│   ├── pages/
│   │   ├── CaptainHome.jsx
│   │   ├── CaptainLogout.jsx
│   │   ├── CaptainProtectWrapper.jsx
│   │   ├── CaptainRiding.jsx
│   │   ├── CaptainSignup.jsx
│   │   ├── CaptainLogin.jsx
│   │   ├── Home.jsx
│   │   ├── Riding.jsx
│   │   ├── Start.jsx
│   │   ├── UserLogin.jsx
│   │   ├── UserLogout.jsx
│   │   └── UserSignup.jsx
│   ├── App.css
│   ├── App.jsx
│   ├── index.jsx
│   └── vite.config.js
├── package.json
└── package-lock.json```

## Components
The `components` folder contains reusable UI components that are used throughout the application. Here are some key components:

- **CaptainDetails.jsx**: Displays details about the captain (driver).
- **ConfirmRide.jsx**: Component for confirming a ride.
- **FinishRide.jsx**: Displays information when a ride is finished.
- **LiveTracking.jsx**: Shows real-time tracking of the ride.
- **LocationSearchPanel.jsx**: Allows users to search for pickup and drop-off locations.
- **RidePopUp.jsx**: Displays a pop-up for ride-related actions.
- **VehiclePanel.jsx**: Shows vehicle details for the ride.
- **LookingForDriver.jsx**: Shows a loading screen while searching for available drivers.
- **WaitingForDriver.jsx**: Displays waiting status after driver is assigned.
- **ConfirmRidePopUp.jsx**: Pop-up dialog for final ride confirmation.

## Context
The `context` folder contains React Context providers that manage global state:

- **UserContext.jsx**: Manages user authentication and profile data.
- **CaptainContext.jsx**: Handles captain (driver) related state.
- **SocketContext.jsx**: Manages WebSocket connections for real-time features.

## Pages
The `pages` folder contains the main route components of the application:

- **Start.jsx**: Landing page for the application.
- **Home.jsx**: Main dashboard for users.
- **UserLogin.jsx**: User login page.
- **UserSignup.jsx**: User registration page.
- **UserLogout.jsx**: Handles user logout.
- **Riding.jsx**: Main ride tracking page for users.
- **CaptainHome.jsx**: Dashboard for captains/drivers.
- **CaptainLogin.jsx**: Captain login page.
- **CaptainSignup.jsx**: Captain registration page.
- **CaptainLogout.jsx**: Handles captain logout.
- **CaptainRiding.jsx**: Ride management page for captains.
- **CaptainProtectWrapper.jsx**: Route protection wrapper for captain routes.

## Routing
The application uses React Router for navigation. The main routing structure is defined in `App.jsx`:

- `/`: Landing page
- `/home`: User dashboard
- `/login`: User login
- `/signup`: User registration
- `/riding`: Active ride page
- `/captain`: Captain routes
  - `/captain/home`: Captain dashboard
  - `/captain/login`: Captain login
  - `/captain/signup`: Captain registration
  - `/captain/riding`: Captain's active ride view

Protected routes ensure that only authenticated users can access certain pages.

## Styling
The application's styling is implemented using:

- **App.css**: Global styles and CSS variables
- **Tailwind CSS**: Utility-first CSS framework for responsive design
- **Material-UI Components**: Pre-built React components with Material Design
- **Custom CSS Modules**: Component-specific styles

Key styling features:
- Responsive design that works across desktop and mobile devices
- Consistent color scheme and typography
- Interactive animations for better user experience
- Dark mode support
- Custom styled components for ride-related UI elements

The styling approach combines the flexibility of Tailwind CSS with the structure of Material-UI components, allowing for both rapid development and customized designs.

Developed by Mousam44. Feel free to reach out at mousambarui@gmail.com for any questions or suggestions.