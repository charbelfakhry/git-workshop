# Node.js with MySQL Project

## 📌 Overview
This project is a **Node.js** application that interacts with a **MySQL** database. It follows best practices for structuring a backend service and includes database management, RESTful API development, and authentication.

## 🛠 Prerequisites
Ensure you have the following installed on your system:
- [Node.js](https://nodejs.org/) (v16 or later recommended)
- [MySQL](https://www.mysql.com/) (v8.0 or later recommended)
- [Postman](https://www.postman.com/) (for API testing, optional)

## 📂 Project Structure
```
/project-root
│── src
│   ├── config          # Configuration files (DB, dotenv, etc.)
│   ├── controllers     # Business logic for API endpoints
│   ├── models          # Database models and schema
│   ├── routes          # Express routes
│   ├── middleware      # Authentication, validation, etc.
│   ├── utils           # Utility functions
│── .env                # Environment variables
│── package.json        # Dependencies and scripts
│── server.js           # Entry point of the application
```

## 🚀 Installation & Setup
1. **Clone the repository**
   ```sh
   git clone https://github.com/charbelfakhry/git-workshop.git
   cd project-root
   ```

2. **Install dependencies**
   ```sh
   npm install
   ```

3. **Configure environment variables**
   Create a `.env` file in the root directory and add the following:
   ```env
   PORT=3000
   DB_HOST=localhost
   DB_USER=root
   DB_PASSWORD=yourpassword
   DB_NAME=mydatabase
   ```

4. **Start MySQL and create a database**
   ```sql
   CREATE DATABASE mydatabase;
   ```

5. **Run database migrations (if applicable)**
   ```sh
   npm run migrate
   ```

6. **Start the server**
   ```sh
   npm start
   ```
   The server will run on `http://localhost:3000`.

## 📌 API Endpoints
### User Routes
| Method | Endpoint        | Description         |
|--------|----------------|---------------------|
| GET    | /users         | Get all users      |
| GET    | /users/:id     | Get user by ID     |
| POST   | /users        | Create a new user  |
| PUT    | /users/:id     | Update user        |
| DELETE | /users/:id     | Delete user        |

## 🛠 Technologies Used
- **Node.js** - Backend runtime
- **Express.js** - Web framework
- **MySQL** - Relational database
- **Sequelize** - ORM for database management
- **dotenv** - Environment variable management
- **bcrypt.js** - Password hashing

## 🔍 Best Practices Followed
✔️ Follows MVC architecture  
✔️ Uses environment variables for security  
✔️ Implements error handling and validation  
✔️ Uses async/await for better promise handling

## 📝 License
This project is licensed under the MIT License.

---
Feel free to contribute by opening issues or submitting pull requests! 🚀
