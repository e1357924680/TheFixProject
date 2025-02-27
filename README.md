# Project Name: The Fix Project

## Overview

The Fix Project is a mobile-first web application designed for users to mark their availability and participate in group activity planning. It is built with React for the frontend and Node.js with MongoDB (Atlas) for the backend.

## Features

- **User Authentication**: Users can sign up and log in.
- **Availability Selection**: Users can mark when they will be home.
- **Activity Suggestion & Voting**: Users can propose activities and vote for the best.
- **Mobile-First UI**: Designed for optimal mobile usability using Bootstrap.

## Tech Stack

- **Frontend**: React, React Icons, Bootstrap
- **Backend**: Node.js, Express, MongoDB Atlas
- **Database**: MongoDB (hosted on Atlas)

## Installation & Setup

### Prerequisites

Make sure you have the following installed:

- [Node.js](https://nodejs.org/)
- [MongoDB Atlas Account](https://www.mongodb.com/cloud/atlas/register)

### Backend Setup

1. Navigate to the `backend` directory:
   ```sh
   cd backend
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Create a `.env` file and configure the following environment variables:
   ```env
   MONGO_URI=your_mongodb_atlas_connection_string
   JWT_SECRET=your_jwt_secret
   PORT=5000
   ```
4. Start the backend server:
   ```sh
   npm start
   ```

### Frontend Setup

1. Navigate to the `frontend` directory:
   ```sh
   cd frontend
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Create a `.env` file and configure the API URL:
   ```env
   REACT_APP_API_URL=http://localhost:5000
   ```
4. Start the frontend server:
   ```sh
   npm start
   ```

## How to Use

1. Register or log in.
2. Click the "I'm going to be home" button to select your availability.
3. Suggest activities and vote on them.
4. Participate in the planned activities.

## Customizing for Your Needs

- Modify `MONGO_URI` in `.env` to use a custom MongoDB instance.
- Change UI styles in `frontend/src/styles`.
- Update backend logic in `backend/routes`.

## Deployment

For production, consider deploying the frontend to Vercel/Netlify and the backend to a cloud provider like Render/Heroku.

## Troubleshooting

- Ensure the backend is running before starting the frontend.
- Check `.env` configurations if the connection fails.
- Run `npm run dev` in the backend for auto-restart on code changes.

---

This document serves as a guide to setting up and running The Fix Project on a local or production environment.
