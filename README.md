# Book Search Engine Starter Code
This project is a book search engine that allows users to search for books using the Google Books API. Users can create an account, log in, and save their favorite books. The application is built with the MERN stack (MongoDB, Express.js, React, Node.js) and utilizes GraphQL with Apollo Server to handle API requests.

## Table of Contents
Installation
Usage
Features
Technologies Used
Contributing
License
Contact

## Installation
### Prerequisites
    Node.js
    npm (Node Package Manager)
    MongoDB
## Steps
### Clone the repository:

    git clone https://github.com/Rualexandra/Book-Search-Engine.git
### Change directory to the project folder:

    cd Book-Search-Engine
### Install server dependencies:

    cd server
    npm install

### Install client dependencies:

    cd ../client
    npm install

### Create a .env file in the server directory and add your MongoDB connection string and JWT secret:


MONGODB_URI=<your-mongodb-connection-string>
SECRET=<your-jwt-secret>

## Usage
Running the Application
### Start the backend server:

    cd server
    npm start

### Start the frontend client:

cd ../client
npm start
Open your browser and navigate to http://localhost:3000.

## Testing GraphQL API
To test the GraphQL API, you can use Apollo GraphQL Playground:

    Navigate to http://localhost:3001/graphql.
### Use the following query to log in and obtain a JWT token:
    
    mutation login($email: String!, $password: String!) {
    login(email: $email, password: $password) {
    token
    user {
      _id
      username
        }
    }
    }
## Provide the required variables in the variables section:

    {
    "email": "your-email@example.com",
    "password": "your-password"
    }
Use the obtained token in the headers to test authenticated queries and mutations.
## Features
    User authentication with JWT
    Search for books using Google Books API
    Save and view favorite books
    Responsive UI built with React and React Bootstrap
## Technologies Used
    Frontend: React, Apollo Client, React Bootstrap
    Backend: Node.js, Express.js, Apollo Server, MongoDB, Mongoose
    GraphQL: Apollo Server, GraphQL
    Authentication: JWT


## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Contact
Author: Alexandra Ruiz
Email: Rualexandra99@gmail.com
GitHub: https://github.com/Rualexandra?tab=repositories 
