# Task Management Web Application

This is a simple Task Management Web Application with a full-stack implementation using Java Spring Boot for the backend and React for the frontend.

## Backend (Java Spring Boot)

### Prerequisites
- Java 8 or higher
- Maven
- MySQL (or another database of your choice)

### Setup
1. Clone the repository: `git clone https://github.com/Knightfury62/Task-Management`
2. Navigate to the `backend` directory: `cd backend`
3. Open the `src/main/resources/application.properties` file and configure your database settings.
4. Run the application: `mvn spring-boot:run`

**Don't Forget**
The backend server should be running on http://localhost:8081

#### API Endpoints

- **GET /tasks**: Fetch all tasks.
- **GET /tasks/{id}**: Fetch a single task by ID./You can try in search Bar By http://localhost:8081/{id}.
- **POST /tasks**: Add a new task.
- **PUT /tasks/{id}**: Update a task by ID.
- **DELETE /tasks/{id}**: Delete a task by ID.

## Frontend (React)

### Prerequisites
- Node.js
- npm (Node Package Manager)

### Setup
1. Navigate to the `frontend` directory: `cd frontend`
2. Install dependencies: `npm install`
3. Start the application: `npm start`

The frontend should be accessible on http://localhost:3000.

#### Views/Pages

- **List View**: Display all tasks with the ability to delete a task.
- **Details View**: Display details of a single task.
- **Add/Edit View**: A form to add a new task or edit an existing one.

#### Connecting Frontend to Backend

- The frontend is configured to connect to the backend at http://localhost:8081. If your backend is running on a different port or domain, update the `REACT_APP_API_BASE_URL` in the `.env` file.

## Database

- The application uses MySQL as the default database. You can change the database configuration in the `application.properties` file.

### Additional Notes

- Make sure both the backend and frontend are running concurrently for the full application experience.
- Customize and extend the application based on your specific requirements.

Enjoy using your Task Management Web Application!
