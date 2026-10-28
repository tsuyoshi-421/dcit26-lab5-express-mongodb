# DCIT 26 Lab 5: Student Records API

REST API for student records built with Node.js, Express, MongoDB, and Mongoose.

## Setup
1. Clone the repository
2. Run `npm install`
3. Copy `.env.example` to `.env`
4. Set your values in `.env`

## MongoDB Configuration
Local installation:

```
MONGODB_URI=mongodb://127.0.0.1:27017/lab5_students
PORT=5000
```

Make sure the MongoDB service is running before starting the server.

## Run the Server
- Development (nodemon): `npm run dev`
- Production: `npm start`

## API Routes
| Method | Route | Description |
|--------|-------|-------------|
| GET | /api/health | Health check |
| GET | /api/students | Get all students |
| GET | /api/students/:id | Get one student (404 if missing) |
| POST | /api/students | Create a student (201) |
| PUT | /api/students/:id | Update a student |
| DELETE | /api/students/:id | Delete a student |

## Sample Request Body
```json
{
  "fullName": "Maria Reyes",
  "course": "BSCS",
  "yearLevel": 1,
  "section": "CS-1B"
}
```