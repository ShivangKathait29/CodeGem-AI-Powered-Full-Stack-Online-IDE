# CodeGem – AI-Powered Full-Stack Online IDE

A **comprehensive browser-based IDE** that enables developers to write, compile, and execute code in multiple programming languages without the need for any local setup.
CodeGem offers a seamless **full-stack development experience** with real-time code execution, intuitive project management, and the foundation for **AI-powered coding assistance**.

---

## ✨ Features

### 💻 Full-Stack Online IDE

* Real-time code writing, compilation, and execution directly in the browser
* Multi-language support with syntax highlighting and auto-completion
* AI-assisted development capabilities (planned for future releases)

### 📂 Project Management

* Create, save, and delete projects securely
* Organize code files for different programming languages
* Persistent storage of user projects using a secure backend

### 🔐 User Authentication

* Secure sign-up and login functionality
* Password hashing and JWT-based authentication
* Session handling with cookies

### 🎨 Modern UI/UX

* VS Code–like editing experience powered by **Monaco Editor**
* Responsive design with **Tailwind CSS**
* Smooth navigation using **React Router DOM** and interactive notifications with **React Hot Toast**

---

## 🏗️ Architecture

### Tech Stack

**Frontend**

* **React** – Building dynamic user interfaces
* **Vite** – Lightning-fast development and bundling
* **Tailwind CSS** – Utility-first styling for rapid UI design
* **Monaco Editor** – Browser-based code editor with advanced features
* **React Router DOM** – Client-side routing
* **Axios** – Simplified HTTP requests
* **React Icons & React Hot Toast** – UI enhancements and notifications

**Backend**

* **Node.js** – JavaScript runtime for server-side development
* **Express.js** – Fast and minimalist web framework
* **MongoDB** – NoSQL database for project and user data
* **Mongoose** – ODM for MongoDB
* **bcryptjs** – Password hashing for secure authentication
* **jsonwebtoken (JWT)** – Token-based authentication
* **cookie-parser** – Handling cookies in HTTP requests
* **cors, http-errors, morgan, debug** – Middleware for CORS, error handling, and logging

---

## 📁 Project Structure

```
CodeGem-AI-Powered-Full-Stack-Online-IDE/
├── backend/
│   ├── bin/
│   │   └── www                  # App entry point
│   ├── models/                  # Mongoose schemas
│   │   ├── projectModel.js
│   │   └── userModel.js
│   ├── routes/                  # API routes
│   │   ├── index.js
│   │   └── users.js
│   ├── app.js                   # Express app configuration
│   ├── package.json
│   └── package-lock.json
├── frontend/
│   ├── public/
│   │   └── vite.svg
│   ├── src/
│   │   ├── components/          # Reusable React components
│   │   │   ├── EditiorNavbar.jsx
│   │   │   ├── GridCard.jsx
│   │   │   ├── ListCard.jsx
│   │   │   └── Navbar.jsx
│   │   ├── images/
│   │   │   ├── authPageSide.png
│   │   │   └── logo.png
│   │   ├── pages/               # App pages
│   │   │   ├── Editior.jsx
│   │   │   ├── Home.jsx
│   │   │   ├── Login.jsx
│   │   │   ├── NoPage.jsx
│   │   │   └── SignUp.jsx
│   │   ├── App.jsx
│   │   ├── helper.js
│   │   ├── main.jsx
│   │   ├── App.css
│   │   ├── index.css
│   │   └── vite.config.js
│   ├── index.html
│   ├── package.json
│   ├── package-lock.json
│   ├── postcss.config.js
│   └── tailwind.config.js
├── .gitignore
└── README.md
```

---

## 🚀 Getting Started

### Prerequisites

* **Node.js** v18+
* **MongoDB** database (local or cloud-based)

### Installation

1️⃣ **Clone the repository**

```bash
git clone https://github.com/ShivangKathait29/CodeGem-AI-Powered-Full-Stack-Online-IDE.git
cd CodeGem-AI-Powered-Full-Stack-Online-IDE
```

2️⃣ **Install dependencies**

```bash
# For backend
cd backend
npm install

# For frontend
cd ../frontend
npm install
```

3️⃣ **Configure Environment Variables**

Create a `.env` file inside the **backend/** directory:

```env
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
PORT=5000
```

4️⃣ **Run the application**

```bash
# Start backend server
cd backend
npm start

# Start frontend development server
cd ../frontend
npm run dev
```

Open your browser at **[http://localhost:5173](http://localhost:5173)** (Vite default) to access the frontend.

---

## 🔧 Key Features in Detail

### Real-Time Compilation & Execution

* Write and run code instantly without installing compilers locally
* Ideal for quick testing and learning multiple languages

### Project Management

* Securely create, save, and retrieve coding projects
* Manage multiple projects with ease

### User Authentication

* JWT-based secure authentication
* Passwords hashed using bcrypt for enhanced security

### AI-Powered Assistance *(Upcoming)*

* Intelligent code completion and debugging support
* Smart recommendations for code optimization

---

## 📈 Future Roadmap

* 🤖 **AI-assisted code generation** and real-time debugging
* 🌐 **Multi-language runtime support** for advanced languages
* 💾 **Cloud-based persistent project storage** with version control
* 🧩 **Collaborative coding** with live sharing and pair programming features

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repo
2. Create a feature branch: `git checkout -b feature/your-feature`
3. Commit changes: `git commit -m 'Add your feature'`
4. Push to the branch: `git push origin feature/your-feature`
5. Open a Pull Request

---

## 📝 License

This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

* **React** & **Vite** for the modern frontend development experience
* **Monaco Editor** for providing a VS Code-like editor inside the browser
* **Node.js**, **Express**, and **MongoDB** for powering the backend
* Open-source community for libraries and tools that make full-stack development seamless
