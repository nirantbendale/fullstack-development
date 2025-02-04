# Multiplication Calculator

A web application for multiplying two numbers and storing results in a MySQL database.

## Setup Instructions

1. Install dependencies:
   ```bash
   # Frontend
   cd frontend
   npm install

   # Backend
   cd ../backend
   npm install
   ```

2. Set up MySQL database:
   ```sql
   CREATE DATABASE multiplication_db;
   USE multiplication_db;
   CREATE TABLE calculations (
       id INT AUTO_INCREMENT PRIMARY KEY,
       number1 INT NOT NULL,
       number2 INT NOT NULL,
       result INT NOT NULL,
       created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
   );
   ```

3. Update backend/.env with your database credentials

4. Start the application:
   ```bash
   # Start backend (from backend directory)
   npm start

   # Start frontend (from frontend directory)
   npm start
   ```

5. Open http://localhost:3000 in your browser