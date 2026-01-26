Todos Application

A RESTful backend application built using Node.js and Express that allows users to manage a list of todos with support for filtering, updating, and deleting tasks stored in a SQLite database.

🚀 Features

Create, read, update, and delete todos

Filter todos by status, priority, and search text

Dynamic query handling based on request parameters

Persistent data storage using SQLite

REST API architecture

🛠️ Tech Stack

Node.js

Express.js

SQLite

JavaScript (

more

Got you 👍 here’s the complete + detailed README.md for the Todos Application, continuing and expanding properly (same quality as your other READMEs).

Todos Application

A RESTful backend application built using Node.js and Express that enables users to manage todos efficiently with full CRUD operations and advanced filtering capabilities. The application uses SQLite for persistent data storage.

🚀 Features

Add new todos

View all todos

Filter todos by status, priority, and search keyword

Retrieve a specific todo by ID

Update todo details (status, priority, or description)

Delete a todo

Dynamic query handling based on request parameters

🛠️ Tech Stack

Node.js

Express.js

SQLite

JavaScript (ES6)

📂 Project Structure
.
├── app.js
├── todoApplication.db
├── package.json
└── package-lock.json

📌 API Endpoints
Get Todos

GET /todos/

Query Parameters:

search_q – search text

status – todo status (TO DO / IN PROGRESS / DONE)

priority – todo priority (HIGH / MEDIUM / LOW)

Supports combined and individual filters.

Get Todo by ID

GET /todos/:todoId/

Returns details of a specific todo.

Create Todo

POST /todos/

Request Body:

{
  "id": 1,
  "todo": "Learn Node.js",
  "priority": "HIGH",
  "status": "IN PROGRESS"
}


Response:

Todo Successfully Added

Update Todo

PUT /todos/:todoId/

Allows updating one field at a time:

todo

priority

status

Response Messages:

Todo Updated

Priority Updated

Status Updated

Delete Todo

DELETE /todos/:todoId/

Deletes the specified todo.

⚙️ Key Concepts Used

RESTful API design

Express routing

Query parameters handling

Dynamic SQL queries

CRUD operations

Async/Await

SQLite database operations

▶️ How to Run Locally
git clone <repository-url>
cd todos-application
npm install
node app.js


Server will start at:

http://localhost:3000/

📌 Future Enhancements

Input validation for todo fields

Pagination for large todo lists

Authentication and authorization

Use prepared statements to prevent SQL injection

Deployment to cloud platforms
