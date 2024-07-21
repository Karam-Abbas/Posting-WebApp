# Posting WebApp

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [API Documentation](#api-documentation)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Introduction
This is a backend project built using Node.js and Express. It provides a basic setup for user registration, authentication, and simple post management.

## Features
- User Registration and Authentication
- User Login and Logout
- Profile Page with User's Posts
- Post Creation, Editing, and Liking
- Protected Routes using JWT

## Technologies Used
- **Node.js**: JavaScript runtime environment
- **Express**: Web framework for Node.js
- **MongoDB**: NoSQL database
- **Mongoose**: MongoDB object modeling tool
- **bcrypt**: Password hashing function
- **jsonwebtoken**: JSON Web Token implementation
- **EJS**: Embedded JavaScript templating
- **cookie-parser**: Parse cookies
- **multer**: Middleware for handling multipart/form-data

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- MongoDB (v4 or higher)

### Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/yourprojectname.git
    ```
2. Navigate to the project directory:
    ```bash
    cd yourprojectname
    ```
3. Install dependencies:
    ```bash
    npm install
    ```
4. Set up environment variables by creating a `.env` file based on the `.env.example`:
    ```bash
    cp .env.example .env
    ```
5. Start the MongoDB server:
    ```bash
    mongod
    ```
6. Start the development server:
    ```bash
    npm start
    ```

## Usage
- **Register a new user**: Navigate to `/` and fill out the registration form.
- **Login**: Navigate to `/login` and provide your credentials.
- **Profile**: After logging in, navigate to `/profile` to view your profile and posts.
- **Create Post**: Use the post form on the profile page to create a new post.
- **Edit Post**: Click the edit link on your post to update its content.
- **Like Post**: Click the like link on a post to like or unlike it.

## API Documentation

### Register a new user
```
POST /register
```
#### Request Body
```json
{
  "email": "user@example.com",
  "username": "username",
  "name": "User Name",
  "age": 25,
  "password": "password"
}
```

### Login
```
POST /login
```
#### Request Body
```json
{
  "email": "user@example.com",
  "password": "password"
}
```

### Create Post
```
POST /post
```
#### Request Body
```json
{
  "content": "This is a new post."
}
```

### Edit Post
```
POST /edit/:id
```
#### Request Body
```json
{
  "content": "Updated post content."
}
```

### Like Post
```
GET /like/:id
```

## Contributing
1. Fork the repository
2. Create a new branch (`git checkout -b feature-branch`)
3. Make your changes
4. Commit your changes (`git commit -m 'Add some feature'`)
5. Push to the branch (`git push origin feature-branch`)
6. Create a new Pull Request

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact
For any questions or feedback, please contact:
- Email: karamabbas03@gmail.com
- GitHub: [Karam-Abbas](https://github.com/Karam-Abbas)
- LinkedIn: [Karam Abbas](https://www.linkedin.com/in/karam-abbas-8884952b8/)
