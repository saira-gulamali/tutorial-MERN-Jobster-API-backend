# 06 - Jobster API Backend

Taken from John Smilga - Node Course - Section 10 - Jobster API

## Description

Full stack App (API and React frontend) providing data for Jobs, with authenticated/protected routes.

This app is built ontop of and has additional filter, sort and pagination functionality. It also uses mongoDB aggregation pipeline to provide stats.

This repo contains the backend only. For the frontend repo, refer to https://github.com/saira-gulamali/tutorial-MERN-Jobster-API-frontend

## Tech stack

### backend

- node
- express
- mongoose
- mongoDB
- nodemon
- express-async-errors
- express-rate-limit
- dotenv
- cors
- bcryptjs
- helmet
- http-status-codes
- jsonwebtoken
- moment
- rate-limiter
- swagger-ui-express
- xss-clean

## Usage

### backend

- npm install

- configure .env file with PORT, MONGO_URI & JWT_SECRET, JWT_LIFETIME, CORS & TESTUSER_ID

* PORT is the port the backend API server will run on
* MONGO_URI is the mongoDB database connection string (ensure to include the database name, username and password)
* JWT_SECRET is a 256-bit encryption key
* JWT_LIFETIME can be set to 30d
* CORS is the url of the frontend server
* TESTUSER_ID is the mongoDB userId of the demo test user in the database (register a user called testUser@test.com and copy the user Id to the .env file)

- npm start
- connect with frontend

#### Models

- /models/User.js
- /models/Job.js

#### Routers

- /routes/auth.js
- /routes/jobs.js
