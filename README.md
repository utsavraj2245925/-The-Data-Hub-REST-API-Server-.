📊 The Data Hub – REST API Server
The Data Hub is a RESTful API server built using Node.js and Express.js as part of the Week 9 Fullstack Development Mission of the internship program.
This project demonstrates how to build a backend server that can handle HTTP requests, manage data, implement CRUD operations, use middleware, and simulate authentication.
Instead of consuming APIs, this project focuses on building APIs from scratch, which is a core skill for modern full-stack development.
🚀 Project Objective
The objective of this project is to build a fully functional REST API server that:
Handles HTTP requests
Implements CRUD operations
Stores data in a mock database
Uses middleware for request logging
Simulates user authentication
🛠 Tech Stack
Node.js
Express.js
JavaScript (ES6)
Postman / Thunder Client (for API testing)
📂 Project Structure
Copy code

data-hub-api/
│
├── server.js
├── package.json
└── README.md
⚙️ Installation & Setup
1️⃣ Clone the repository
Bash
Copy code
git clone https://github.com/your-username/data-hub-api.git
2️⃣ Navigate to the project folder
Bash
Copy code
cd data-hub-api
3️⃣ Install dependencies
Bash
Copy code
npm install
4️⃣ Start the server
Bash
Copy code
node server.js
The server will run on:
Copy code

http://localhost:5000
🌐 API Endpoints
Blog Routes
Get All Posts
Copy code

GET /posts
Returns all blog posts.
Get Single Post
Copy code

GET /posts/:id
Returns a specific blog post by ID.
Create New Post
Copy code

POST /posts
Request Body Example:
Json
Copy code
{
  "title": "My First Blog",
  "content": "This is my blog post"
}
Update Post
Copy code

PUT /posts/:id
Updates an existing post.
Delete Post
Copy code

DELETE /posts/:id
Removes a post from the database.
🗄 Mock Database
This project uses a simple in-memory array to simulate a database.
Javascript
Copy code
let blogPosts = [];
Each blog post is stored as an object:
Javascript
Copy code
{
  id: 1,
  title: "Example Title",
  content: "Example Content"
}
🧩 Custom Middleware
A custom middleware function logs each incoming request to the console.
Example output:
Copy code

[GET] /posts - 10:05 AM
[POST] /posts - 10:07 AM
This helps developers monitor API activity.
🔐 Fake Authentication Route
A mock authentication endpoint is implemented.
Login Route
Copy code

POST /login
Request Body:
Json
Copy code
{
  "username": "admin",
  "password": "1234"
}
Response Example:
Json
Copy code
{
  "token": "fake-jwt-token-123456"
}
This simulates how authentication works in real backend systems.
🧪 API Testing
All API endpoints were tested using:
Postman
Thunder Client (VS Code extension)
Tests include:
Creating posts
Fetching posts
Updating posts
Deleting posts
Testing login authentication
📈 Learning Outcomes
By completing this project, the following backend development concepts were learned:
Creating servers using Node.js and Express
Building RESTful APIs
Implementing CRUD operations
Writing custom middleware
Handling HTTP requests and responses
Testing APIs using Postman
Understanding basic authentication concepts
🎯 Internship Mission
This project is part of the Week 9 Mission of the internship program where interns transition from frontend development to fullstack development.
The goal is to understand how frontend applications communicate with backend servers using REST APIs.
👨‍💻 Author
Utsav Raj
B.Tech CSE (AIML) – Final Year
Fullstack Developer Intern
GitHub:
https://github.com/utsavraj2245925⁠�
⭐ Acknowledgement
Thanks to the internship program for providing hands-on experience in real-world backend development and API creation.
