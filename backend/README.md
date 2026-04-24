# Backend API Automated Tests
**Author:** Nave Dan (QA)

This directory contains automated End-to-End (E2E) and integration tests for the MeetDrop backend API endpoints. The scripts utilize native Node.js asynchronous `fetch` and `http` requests to validate routing, database operations, and error handling without requiring external frameworks.

## How to Run Tests
Ensure the backend server is running locally on `http://localhost:5000`.

Open your terminal, navigate to the `backend/` directory, and run any of the following commands:

* `node test_auth.js` - Validates user registration, standard login, and Admin token generation.
* `node test_login.js` - Validates basic login request formatting and timeout handling using native HTTP requests.
* `node test_match.js` - Validates the stateless concurrent matchmaking algorithm.
* `node test_users.js` - Validates data integrity for user profiles, favorites toggling, and history visibility.
