
# My Express.js REST API

A simple Express.js app demonstrating routing, 404 handling, and error middleware.

##  Setup Instructions

bash
git clone <your-repo-url>
cd my-express-app
npm install
npm start
`

Server will run at `http://localhost:5000`

---

## 📌 Available Routes

### 1. `GET /items`

Returns a hello world message.

**Request:**

http
GET /items HTTP/1.1
Host: localhost:5000


**Response:**

json
{
  "message": "Hello World!"
}


---

### 2. `GET /itemserror`

Simulates a server error.

**Request:**

http
GET /items HTTP/1.1
Host: localhost:5000


**Response:**

json
{
  "error": "Intentional server error",
  "status": 500
}


---

### 3. Invalid Route Example

**Request:**

http
GET /items/unknown HTTP/1.1
Host: localhost:5000


**Response:**

json
{
  "error": "Route not found",
  "status": 404,
  "path": "/items/unknown"
}


---

## 🧪 Testing with Postman

1. Open Postman
2. Use `GET http://localhost:5000/items`
3. Test `GET http://localhost:5000/itemserror` for error handling
4. Test any unknown route like `GET http://localhost:5000/items/404test`



## 🛠 Built With

* Node.js
* Express.js

