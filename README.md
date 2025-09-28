# Full-Stack-Online-Code-IDE
Project Scope
CodeGem-AI-Powered-Full-Stack-Online-IDE is a full-stack online IDE that allows users to write, compile, and execute code in various programming languages directly in their browser. It provides features like real-time code editing, a responsive UI, and potentially AI-powered functionalities (though the specific AI features are not immediately clear from the provided files). The project aims to offer a comprehensive development environment for users, with authentication, project management, and a rich code editing experience.

Tech Stack
The project is built with a MERN (MongoDB, Express.js, React, Node.js) stack, along with additional libraries and tools for a complete online IDE experience.

Backend:

Node.js/Express.js: The core backend framework, handling API routes, authentication, and communication with the database.
express: Web framework for Node.js.
http-errors: HTTP error creation.
morgan: HTTP request logger middleware.
cookie-parser: Middleware to parse cookies.
cors: Enables Cross-Origin Resource Sharing.
Database:
mongoose: MongoDB object modeling for Node.js. Used for userModel.js and projectModel.js to define schemas and interact with the MongoDB database.
Authentication & Security:
bcryptjs: For hashing passwords.
jsonwebtoken: For creating and verifying JWT tokens for user authentication.
Templating Engine:
ejs: Embedded JavaScript templating for server-side rendering (though primarily an API backend, it might be used for error pages or simple server-rendered views).
Frontend:

React: The core JavaScript library for building user interfaces.
react-router-dom: For client-side routing within the React application.
Build Tool:
Vite: A fast build tool that provides a rapid development experience.
Styling:
tailwindcss: A utility-first CSS framework for rapid UI development.
postcss: A tool for transforming CSS with JavaScript plugins.
Code Editor:
@monaco-editor/react: A React wrapper for the Monaco Editor (the same editor that powers VS Code), providing advanced code editing features, syntax highlighting, and language support.
Icon Library:
react-icons: A collection of popular SVG icon packs as React components.
Utility Libraries:
axios: A promise-based HTTP client for making API requests to the backend.
js-cookie: A simple, lightweight JavaScript API for handling browser cookies.
Other Tools:

ESLint: For linting and maintaining code quality.
Project Structure:
CodeGem-AI-Powered-Full-Stack-Online-IDE/
├── backend/                      # Express.js backend
│   ├── models/                    # Mongoose models
│   │   ├── projectModel.js        # Schema for project data
│   │   └── userModel.js           # Schema for user data
│   ├── routes/                    # API route definitions
│   │   ├── index.js               # Main route entry point
│   │   └── users.js               # User-related routes
│   ├── app.js                     # Express app configuration
│   ├── package.json               # Backend dependencies & scripts
│   └── package-lock.json          # Exact backend dependency versions
│
├── frontend/                      # React + Vite frontend
│   ├── src/                       # Frontend source code
│   │   ├── components/            # Reusable UI components
│   │   │   ├── EditiorNavbar.jsx  # Navbar for the code editor page
│   │   │   ├── GridCard.jsx       # Grid-style card component
│   │   │   ├── ListCard.jsx       # List-style card component
│   │   │   └── Navbar.jsx         # Main site navigation bar
│   │   ├── pages/                 # Page-level components
│   │   │   ├── Editior.jsx        # Online code editor page
│   │   │   ├── Home.jsx           # Landing/home page
│   │   │   ├── Login.jsx          # User login page
│   │   │   ├── NoPage.jsx         # 404 / Not found page
│   │   │   └── SignUp.jsx         # User sign-up page
│   │   ├── App.jsx                # Root React component
│   │   ├── App.css                # App-level styles
│   │   ├── helper.js              # Frontend utility functions
│   │   ├── index.css              # Global CSS
│   │   └── main.jsx               # React entry point
│   ├── index.html                 # HTML template
│   ├── package.json               # Frontend dependencies & scripts
│   ├── package-lock.json          # Exact frontend dependency versions
│   ├── postcss.config.js          # PostCSS configuration
│   ├── tailwind.config.js         # Tailwind CSS configuration
│   └── vite.config.js             # Vite build configuration
│
├── .gitignore                     # Git ignore rules
└── README.md                      # Project documentation
