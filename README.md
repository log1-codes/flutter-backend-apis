# Express Backend Demo

This is a simple Node.js + Express backend with 4 user APIs for testing with your Flutter app.

## Setup

1. Install dependencies:
   ```bash
   npm install
   ```

2. Start the server:
   ```bash
   npm run dev
   ```
   The server will run on [http://localhost:3000](http://localhost:3000)

## API Endpoints

### 1. List all users
- **GET /users**
- Response: `[ { id, name, email }, ... ]`

### 2. Get user by ID
- **GET /users/:id**
- Example: `/users/1`
- Response: `{ id, name, email }`

### 3. Create a new user
- **POST /users**
- Body (JSON): `{ "name": "Charlie", "email": "charlie@example.com" }`
- Response: `{ id, name, email }`

### 4. Delete a user by ID
- **DELETE /users/:id**
- Example: `/users/1`
- Response: `{ message: "User deleted" }`

---

You can use these endpoints in your Flutter app for testing HTTP requests. 