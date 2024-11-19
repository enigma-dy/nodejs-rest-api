## Getting Started

Follow these instructions to set up the project on your local machine for development and testing purposes.

### Requirements

- Node.js installed
- NPM (Node Package Manager) installed

## Technologies Used

- ![Node.js](https://img.shields.io/badge/Node.js-339933.svg?style=for-the-badge&logo=nodedotjs&logoColor=white): The runtime environment for executing the application.
- ![MongoDB](https://img.shields.io/badge/MongoDB-47A248.svg?style=for-the-badge&logo=mongodb&logoColor=white): A NoSQL database for data persistence.
- ![Mongoose](https://img.shields.io/badge/Mongoose-880000.svg?style=for-the-badge&logo=mongoose&logoColor=white): An ODM (Object Data Modeling) library for MongoDB and Node.js.
- ![JSON Web Token](https://img.shields.io/badge/JSON%20Web%20Tokens-000000.svg?style=for-the-badge&logo=JSON-Web-Tokens&logoColor=white): Used for user authentication.
- ![Express.js](https://img.shields.io/badge/Express-000000.svg?style=for-the-badge&logo=Express&logoColor=white): A web application framework for building RESTful APIs.
- ![JSON](https://img.shields.io/badge/JSON-000000.svg?style=for-the-badge&logo=JSON&logoColor=white): Data interchange format used in the project.
- ![Jest](https://img.shields.io/badge/Jest-C21325.svg?style=for-the-badge&logo=Jest&logoColor=white):JavaScript testing framework ensuring code reliability and simplicity.
- ![Gravatar](https://img.shields.io/badge/Gravatar-1E8CBE.svg?style=for-the-badge&logo=Gravatar&logoColor=white): Global avatar service for user profile images linked to email addresses.

### Installing

1. Clone the repository to your local machine.
   ```bash
   git clone https://github.com/enigma-dy/nodejs-rest-api.git
   ```
1. Navigate to the project folder.
   ```bash
   cd nodejs-rest-api-homework
   ```
1. Install dependencies.
   ```bash
   npm install
   ```

### Running the Application

- **Production Mode:**
  ```bash
  npm start
  ```
- **Development Mode with Nodemon:**
  ```bash
  npm run dev
  ```
- **Running Tests**
  To execute unit tests using Jest, use the following command:
  ```bash
  npm run test
  ```

## Project API Endpoints

### Contact endpoints

- **(GET) `/api/contacts`:** Retrieve a list of all contacts.
- **(GET) `/api/contacts/`:contactId:** Retrieve a specific contact by ID.
- **(POST) `/api/contacts`:** Add a new contact to the list.
- **(PUT) `/api/contacts/`:contactId:** Update an existing contact's information.
- **(PATCH) `/api/contacts/`:contactId/favorite:** Partially update an existing contact's information.
- **(DELETE) `/api/contacts/`:contactId:** Delete an existing contact from the list.

### User endpoints

- **(POST) `/api/users/signup`:** Register a new user.
- **(POST) `/api/users/signin`:** Login and obtain a JWT.
- **(POST) `/api/users/logout`:** Logout the user.
- **(GET) `/api/users/current`:** Retrieve information about the currently logged-in user.
- **(PATCH) `/api/users/avatars`:** Change the user's avatar.
- **(GET) `/api/users/verify/:verificationToken`:** Verify the user's email address using the provided token.
- **(POST) `/api/users/verify`:** Request a second verification email.

### Additional Endpoints

- **(GET) `/api/contacts?page=<page_number>&limit=<page_size>`:** Retrieve paginated contacts.
- **(GET) `/api/contacts?favorite=true`:** Retrieve contacts marked as favorites.
- **(PATCH) `/api/users`:** Update the user's subscription level.
