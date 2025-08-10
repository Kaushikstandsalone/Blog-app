Blog App 📝
A full-stack blogging platform where users can create, edit, delete, and view blog posts.
Built with a modern tech stack for a seamless, responsive, and secure experience.

🚀 Technologies Used
Frontend
React.js – Component-based UI

Material-UI – Prebuilt and customizable UI components

Backend
Node.js – JavaScript runtime environment

Express.js – Web application framework for Node.js

Database
MongoDB – NoSQL database for storing blog data

Authentication
JWT (JSON Web Token) – Secure authentication and authorization

📌 Features
🖋 Create, Edit, and Delete Blogs

🔍 View All Blogs with a responsive UI

🔒 Secure Authentication using JWT

🌐 REST API for CRUD operations

📱 Mobile-Friendly Design

🛠 Installation and Setup
Clone the repository

bash
Copy
Edit
git clone https://github.com/Kaushikstandsalone/Blog-app.git
cd Blog-app
Install dependencies
Frontend:

bash
Copy
Edit
cd client
npm install
Backend:

bash
Copy
Edit
cd ../server
npm install
Set up environment variables
Create a .env file in the server directory:

env
Copy
Edit
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
PORT=5000
Run the app
Backend:

bash
Copy
Edit
npm run server
Frontend:

bash
Copy
Edit
npm start
📂 Project Structure
bash
Copy
Edit
Blog-app/
│
├── client/         # Frontend (React + Material-UI)
├── server/         # Backend (Node.js + Express.js)
└── README.md
