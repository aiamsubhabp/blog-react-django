# Note Taking App

## App Description
A feature-rich note-taking application built with Django for the backend API and React for the frontend. This application provides full CRUD (Create, Read, Update, Delete) capabilities for managing notes and incorporates user authentication with JWT tokens.

## Features
 - **User Authentication**: Secure registration and login using JWT tokens.
 - **CRUD Operations**: Create, read, update, and delete notes.
 - **User-specific Notes**: Users can only see and manage their own notes.
 - **Modern UI**: Clean and intuitive user interface built with React. 

## Prerequisites
 - Python 3.x
 - Node.js & npm
 - Django
 - Vite

## Usage
 - Register a new account or log in with existing credentials
 - Create, edit, or delete notes from your personal dashboard
 - View all of your notes in a user-friendly interface

## API Endpoints
 - User Management:
    - Register: POST /api/user/register/ - Register a new user. Request body should include username, password, and optionally email.
    - Obtain Token: POST /api/token/ - Obtain a JWT token for authentication. Request body should include username and password.
    - Refresh Token: POST /api/token/refresh/ - Refresh an existing JWT token. Request body should include refresh token.

 - Notes Management:
     - List and Create Notes:
        - GET /api/notes/ - Retrieve a list of all notes for the authenticated user.
        - POST /api/notes/ - Create a new note. Request body should include title and content.
     - Delete Note:
        - DELETE /api/notes/delete/<int:pk>/ - Delete a specific note by its ID. 

## License
This project is licensed under the MIT License. See the LICENSE file for details.