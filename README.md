# WTWR (What to Wear?): Back End

The Express API behind WTWR, a weather-based clothing recommendation app. It handles users, clothing items and likes, stores data in MongoDB, and serves the React front end.

- Live API: https://wtwr-backend-gz5j.onrender.com
- Live app: https://wtwr-frontend.vercel.app
- Front-end code: https://github.com/dionshort/wtwr-frontend

> Hosted on Render's free tier, so the first request after a period of inactivity can take up to a minute while the server wakes up.

## Features
- User sign-up and login with JWT authentication
- Create, delete, like and unlike clothing items
- Request validation with Celebrate (Joi), returning clear 400 errors for invalid data
- Centralised error handling with consistent status codes (400, 401, 403, 404, 409, 500)
- Request and error logging with Winston

## Tech stack
Node.js · Express · MongoDB Atlas · Mongoose · Celebrate/Joi · Winston · Render

## Running locally
Create a `.env` file with:
- `MONGODB_URI` - MongoDB connection string
- `JWT_SECRET` - a long random string for signing tokens
- `PORT` - optional, defaults to 3001

`npm run start` - launch the server

`npm run dev` - launch the server with hot reload via nodemon
