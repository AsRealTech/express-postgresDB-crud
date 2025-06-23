Brief Documentation

 🔹 How to Run

1. Clone or download this project.
2. Update `db.js` with your PostgreSQL credentials.
3. Install dependencies:

bash
npm install


4. Start the server:

bash
node index.js

🔹 Test with Postman or curl

*GET* all users:
GET http://localhost:3000/users

*GET* user by ID:
GET http://localhost:3000/users/1

*POST* new user:

json
POST http://localhost:3000/users
{
  "name": "Alice",
  "email": "alice@example.com",
  "age": 25
}

**PUT** update user:

json
PUT http://localhost:3000/users/1
{
  "name": "Alice Updated",
  "email": "alice@newdomain.com",
  "age": 26
}


**DELETE** user:
DELETE http://localhost:3000/users/1
