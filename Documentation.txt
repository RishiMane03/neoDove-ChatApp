ChatApp is a real-time chat application built using Node.js for the backend and React 
for the frontend. It features user authentication and real-time messaging using WebSockets.

FILE STRUCTURE: 
ChatApp/
│
├── Backend/
│   ├── config/
│   │   └── db.js
│   ├── models/
│   │   └── User.js
│   ├── routes/
│   │   ├── auth.js
│   │   └── chat.js
│   ├── controllers/
│   │   ├── authController.js
│   │   └── chatController.js
│   ├── server.js
│   └── package.json
│
└── Frontend/
    ├── public/
    ├── src/
    │   ├── components/
    │   ├── pages/
    │   ├── App.js
    │   ├── index.js
    │   └── package.json


Code Structure:

Backend:
    server.js: Entry point for the Node.js server.
    config/db.js: Database configuration.
    models/User.js: User schema and model.
    routes/auth.js: Routes for user authentication.
    routes/chat.js: Routes for chat functionality.
    controllers/authController.js: Handles authentication logic.
    controllers/chatController.js: Handles chat logic.

Frontend:
    src/index.js: Entry point for the React app.
    src/App.js: Main App component.
    src/components/: React components.
    src/pages/: Page components.

Authentication:
JWT (JSON Web Tokens): Used for user authentication. Tokens are generated during login 
and verified on protected routes.

Bcrypt: Used to hash user passwords before saving them to the database.

WebSockets:
Socket.IO: Used for real-time communication between the server and clients. It handles 
event-based messaging, ensuring users can send and receive messages instantly.