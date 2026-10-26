# Employee App — Assignment 3

## Requirements
- Node.js 18 or newer
- MongoDB Atlas cluster and database user

## Setup
1. In this folder, run `npm install`.
2. Copy `.env.example` to `.env`.
3. Replace the placeholder `MONGODB_URI` with your MongoDB Atlas connection string. Do not commit `.env`.
4. Run `npm start`.
5. Open http://localhost:3000.

The provided `dist/Frontend` files are included unchanged.

## API routes
The backend supports both `/api/employeelist` (assignment route) and `/employeelist` (used by the provided frontend).

- `GET /api/employeelist` — list employees
- `GET /api/employeelist/:id` — get one employee
- `POST /api/employeelist` — add employee; JSON body: `name`, `location`, `position`, `salary`
- `PUT /api/employeelist` — update employee; send `_id` plus `name`, `location`, `position`, `salary`
- `DELETE /api/employeelist/:id` — delete employee

All endpoints are also available without `/api` for compatibility with the supplied frontend.
