# SkillSwap Platform

**SkillSwap** is a peer-to-peer learning platform that allows users to create, join, and manage learning sessions. It includes gamification features like coins, leaderboards, and achievements to make learning engaging and rewarding.

---

## Table of Contents

- [Project Structure](#project-structure)
  - [Frontend (`skillswap/`)](#frontend-skillsswap)
  - [Backend (`server/`)](#backend-server)
  - [Chatbot Backend (`chatbot-backend/`)](#chatbot-backend-chatbot-backend)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
  - [Clone the Repository](#clone-the-repository)
  - [Install Dependencies](#install-dependencies)
  - [Set Up Environment Variables](#set-up-environment-variables)
  - [Running the Project](#running-the-project)
- [How to Use the Platform](#how-to-use-the-platform)
- [API Endpoints](#api-endpoints)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)
- [Note](#note)

---

## Project Structure

### Frontend (`skillswap/`)

Built with **React**, the frontend handles the user interface and experience.

- `src/components/`: Reusable components like `SessionModal`, `Chatbot`, etc.  
- `src/pages/`: Main pages like `Dashboard`, `Profile`, `Leaderboard`, etc.  
- `src/styles/`: CSS files for styling the application.  
- `public/`: Static assets including images and `index.html`.  

### Backend (`server/`)

Built with **Node.js** and **Express**, the backend handles API requests, authentication, and database interactions.

- `server.js`: Entry point of the backend server.  
- `routes/`: API endpoints:
  - `auth.js`: User authentication (signup, login).  
  - `profile.js`: Manage user profiles (view, update).  
  - `session.js`: Manage learning sessions (create, update, delete).  
- `models/`: Database models (e.g., `User.js`).  
- `middleware/`: Middleware like `authMiddleware.js` for JWT authentication.  

### Chatbot Backend (`chatbot-backend/`)

A separate backend integrated with an AI API for automated chatbot responses.

---

## Prerequisites

Ensure you have the following installed:

- **Node.js** (v16 or higher)  
- **npm** (Node Package Manager)  
- **MongoDB** (local or cloud instance)  

---

## Installation

### Clone the Repository

```
git clone https://github.com/AnmolGithubx/StudySwap.git
cd skillswap
```

### Install Dependencies

**Frontend:**

```
cd skillswap
npm install
```

**Backend:**

```
cd ../server
npm install
```

**Chatbot Backend:**

```
cd ../chatbot-backend
npm install
```

### Set Up Environment Variables

Create `.env` files with the following variables:

**Backend (`server/.env`):**

```
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
```

**Chatbot Backend (`chatbot-backend/.env`):**

```
PORT=5001
AI_API_KEY=your_ai_api_key
```

---

## Running the Project

Start each part of the app in separate terminals:

- **Backend Server**

```
cd server
npm start
```

Runs on: [http://localhost:5000](http://localhost:5000)

- **Chatbot Backend**

```
cd ../chatbot-backend
npm start
```

Runs on: [http://localhost:5001](http://localhost:5001)

- **Frontend**

```
cd ../skillswap
npm start
```

Runs on: [http://localhost:3000](http://localhost:3000)

---

## How to Use the Platform

- **Sign Up / Log In:** Create an account or log in.
- **Dashboard:** View stats, achievements, and daily challenges.
- **Learning Sessions:** Create and join sessions using `SessionModal`.
- **Profile Management:** Update bio, skills, and experience.
- **Browse Skills:** Find mentors or learning opportunities.
- **Chatbot:** Get assistance and answers via the AI chatbot.
- **Leaderboards:** Compete based on coins, XP, and sessions attended.

---

## API Endpoints

### Authentication (`/api/auth`)

- `POST /register` – Register a new user
- `POST /login` – Log in and receive a JWT token

### Profile (`/api/profile`)

- `GET /` – Get current user's profile
- `PUT /` – Update user's profile

### Session (`/api/session`)

- `POST /` – Create or update a session
- `DELETE /` – Delete a session

---

## Technologies Used

| Layer         | Technologies                      |
|---------------|---------------------------------|
| Frontend      | React, Axios, React Router       |
| Backend       | Node.js, Express.js, MongoDB, JWT|
| Chatbot       | Node.js, AI API integration      |

---

## Contributing

1. Fork the repository.  
2. Create a new branch.  
3. Commit your changes.  
4. Push to your branch.  
5. Open a pull request.

---

## License

This project is licensed under the MIT License. See the LICENSE file for details.

---

## Contact

- Email: a56231919@gmail.com  

---

## Note

Replace placeholders (`your_mongodb_connection_string`, `your_jwt_secret`, `your_ai_api_key`, and contact info) with actual values.

---

If you want, I can also improve it further with badges, table of contents, and visually separated sections to make it GitHub-ready and more professional.


Made with ❤️ and lots of coffee.
```
