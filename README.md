# Student Portal Management System

A production‑style full‑stack application that enables students, faculty, and administrators to manage academic information.

## Overview
- **Students** can view their profile, attendance, marks, and announcements.
- **Faculty** can record attendance, upload marks, and publish announcements.
- **Administrators** manage users, courses, subjects, and overall system configuration.

The project follows clean‑architecture principles with a layered backend (Controller → Service → DAO) and a modern React front‑end.

## Technology Stack
- **Backend**: Java 21, Spring Boot 3.x, Spring Security, JDBC, MySQL
- **Frontend**: React 19, Vite, JavaScript (ES2023), Axios
- **Build Tools**: Maven, npm
- **Testing**: JUnit 5, Spring Test, React Testing Library

## Prerequisites
- JDK 21
- Maven 3.9+
- Node.js 20+ and npm
- MySQL 8 (or use the embedded H2 for tests)

## Getting Started
```bash
# Clone the repository (if you haven't already)
git clone <repo-url>
cd student-portal-management-system
```

### Backend
```bash
# Navigate to the backend module
cd backend
# Install Maven dependencies and run tests
mvn clean verify
# Package the application
mvn package
# Run the Spring Boot service
java -jar target/spm-backend-0.0.1-SNAPSHOT.jar
```
The API will be available at `http://localhost:8080`.

### Frontend
```bash
# In a new terminal, from the project root:
cd frontend
npm install
npm run dev   # Development server at http://localhost:5173
# Or to build for production:
npm run build
```

## Testing
- Backend unit/integration tests are executed with `mvn test`.
- Frontend tests can be run with `npm test` (Jest + React Testing Library).

## Contribution
Feel free to open issues or submit pull requests. Follow the existing code style and run the full test suite before submitting.

## License
MIT License – see `LICENSE` file for details.