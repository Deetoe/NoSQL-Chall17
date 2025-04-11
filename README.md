# NoSQL: Social Network API

![License](https://img.shields.io/badge/License-MIT-blue.svg)  
<img alt="MongoDB" src="https://img.shields.io/badge/MongoDB-4.4+-green.svg">
<img alt="Express" src="https://img.shields.io/badge/Express-4.17+-green.svg">
<img alt="Mongoose" src="https://img.shields.io/badge/Mongoose-6.0+-green.svg">

## Overview

This project delivers a robust back-end API tailored for a social networking application. Built using MongoDB, Express.js, and Mongoose ODM, the API allows users to post thoughts, react to others’ content, and manage their list of friends. It serves as a demonstration of how NoSQL databases can support dynamic and unstructured data structures often required by social platforms.

## Table of Contents

- [Installation](#installation)  
- [Usage](#usage)  
- [API Endpoints](#api-endpoints)  
- [Contributing](#contributing)  
- [License](#license)  
- [Questions](#questions)

## Installation

To get the project up and running locally, follow these steps:

```bash
# Clone the repository
git clone https://github.com/Deetoe/NoSQL-Chall17.git

# Navigate into the project folder
cd NoSQL-Chall17

# Install dependencies
npm install

# Optional: Build scripts or assets if needed
npm run build

# Start the server
npm start
Usage
Once the server is running, you can interact with the API using tools like Insomnia or Postman to test various endpoints.

The API is hosted at:
http://localhost:3001

API Endpoints
👤 User Routes
GET /api/users – Retrieve all users

GET /api/users/:userId – Get a single user (with their thoughts and friends)

POST /api/users – Add a new user

PUT /api/users/:userId – Modify a user by ID

DELETE /api/users/:userId – Remove a user (also deletes their associated thoughts)

🤝 Friend Routes
POST /api/users/:userId/friends/:friendId – Add a friend

DELETE /api/users/:userId/friends/:friendId – Remove a friend

💬 Thought Routes
GET /api/thoughts – Retrieve all thoughts

GET /api/thoughts/:thoughtId – Get a specific thought by ID

POST /api/thoughts – Create a new thought (linked to a user)

PUT /api/thoughts/:thoughtId – Update a thought

DELETE /api/thoughts/:thoughtId – Delete a thought

🔁 Reaction Routes
POST /api/thoughts/:thoughtId/reactions – Add a reaction to a thought

DELETE /api/thoughts/:thoughtId/reactions/:reactionId – Remove a reaction from a thought

Contributing
Created and maintained by Daniel Gonzalez

License
This project is covered under the MIT License.

Questions
For questions or further information, feel free to reach out:

📧 Email: dannygonzr20@gmail.com
🐙 GitHub: Deetoe