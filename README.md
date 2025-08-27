# 🤝 Collabhub Backend

A powerful backend service for **Collabhub** — a platform designed to connect collaborators seamlessly.  
This backend handles **authentication, friend requests, messaging, and notifications** with a clean and scalable architecture.

---

## 🛠️ Tech Stack
- **Node.js** & **Express.js** – REST API framework  
- **Socket.io** – Real-time communication  
- **Database:** MongoDB  
- **Authentication:** JWT  
- **Environment Management:** dotenv  
- **Other Utilities:** CORS, Nodemon, bcrypt, etc.  

---

## ⚙️ Installation

```bash
1. Clone the repository
   git clone https://github.com/sahil-verma-9696/collabhub-backend.git
   cd collabhub-backend

2. Install dependencies
   npm install

3. Setup environment variables
   # Create a .env file in the root folder and add:
   PORT=5000
   DATABASE_URL=your_mongo_connection_url
   JWT_SECRET=your_secret_key

4. Run the server
   # For development:
   npm run dev

   # For production:
   npm start

---file Structure---
``
└── 📁src
    └── 📁controllers
        └── 📁auth
            ├── login.controller.js
            ├── logout.controller.js
            ├── me.controller.js
            ├── signup.controller.js
        └── 📁module
            ├── createModule.js
        └── 📁task
            ├── createTaskById.js
            ├── deleteTaskById.js
            ├── updateTaskById.js
        └── 📁workspace
            ├── createWorkspace.js
            ├── deleteWorkspcace.js
            ├── getWorkspace.js
            ├── getWorkspaceById.js
            ├── updateWorkspace.js
    └── 📁database
        ├── connection.js
    └── 📁middleware
        ├── authMiddleware.js
        ├── error-handler.js
    └── 📁models
        ├── attachment.model.js
        ├── comment.model.js
        ├── document.model.js
        ├── label.model.js
        ├── message.model.js
        ├── module.model.js
        ├── notification.model.js
        ├── task.model.js
        ├── team.model.js
        ├── user.model.js
        ├── workspace.model.js
    └── 📁routes
        ├── auth.routes.js
        ├── tasks.routes.js
        ├── workspace.routes.js
    └── 📁socket
        └── 📁namespaces
            └── 📁chat
                └── 📁listeners
                    ├── message.js
                    ├── online.js
                    ├── typing-stop.js
                    ├── typing.js
                ├── index.js
            └── 📁root
                ├── index.js
        ├── index.js
    └── 📁utilities
        ├── async-handler.js
        ├── generateToken.js
    ├── rest.js
    └── server.js
``

---🤝 Contributing---
1. Fork the repository

2. Create your feature branch
   git checkout -b feature/YourFeature

3. Commit your changes
   git commit -m "Add some feature"

4. Push to your branch
   git push origin feature/YourFeature

5. Open a Pull Request
