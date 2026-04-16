# freeCodeCamp Advanced Node and Express

## Project Overview
This is a boilerplate for the freeCodeCamp "Advanced Node and Express" curriculum. It covers authentication with Passport.js, real-time communication with Socket.io, and MongoDB integration.

## Architecture
- **Runtime:** Node.js (v20)
- **Framework:** Express.js
- **Template Engine:** Pug
- **Database:** MongoDB (configured via `MONGO_URI` environment variable)
- **Authentication:** Passport.js (local + GitHub strategies)
- **Real-time:** Socket.io
- **Session Store:** connect-mongo

## Project Structure
- `server.js` — Main entry point, Express app setup
- `connection.js` — MongoDB connection utility (do not modify)
- `public/` — Static assets (client.js, style.css)
- `views/pug/` — Pug templates (index, profile, chat)
- `freeCodeCamp/` — FCC testing utilities

## Running the App
- **Dev:** `npm run dev` (nodemon with auto-restart)
- **Production:** `node server.js`
- **Port:** 5000, bound to `0.0.0.0`

## Environment Variables
- `PORT` — Server port (default: 5000)
- `NODE_ENV` — Environment (development/production)
- `MONGO_URI` — MongoDB connection string (required for database features)
- `SESSION_SECRET` — Express session secret

## Key Notes
- `connection.js` should NOT be modified (FCC requirement)
- App listens on `0.0.0.0:5000` for Replit proxy compatibility
- MongoDB URI must be set for database-dependent features to work
