# Blog App

A full-stack blog application built with modern web technologies, featuring user authentication, content management, and a responsive design.

## 🚀 Features

- **User Authentication**: Secure login/register system with JWT tokens
- **Create & Edit Posts**: Rich text editor for creating and managing blog posts
- **Responsive Design**: Mobile-friendly interface built with Material-UI
- **User Profiles**: Personal profiles and user management
- **Search & Filter**: Find posts by keywords, categories, or authors
- **Comments System**: Interactive commenting on blog posts
- **Admin Dashboard**: Content moderation and user management

## 🛠️ Technologies Used

### Frontend
- **React.js** - JavaScript library for building user interfaces
- **Material-UI** - React component library for faster development

### Backend
- **Node.js** - JavaScript runtime environment
- **Express.js** - Web application framework for Node.js

### Database
- **MongoDB** - NoSQL document database

### Authentication
- **JWT (JSON Web Tokens)** - Secure authentication and authorization

## 📋 Prerequisites

Before running this application, make sure you have the following installed:

- [Node.js](https://nodejs.org/) (v14.0.0 or higher)
- [MongoDB](https://www.mongodb.com/) (v4.0 or higher)
- [npm](https://www.npmjs.com/) or [yarn](https://yarnpkg.com/)

## ⚡ Quick Start

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/blog-app.git
cd blog-app
```

### 2. Install dependencies

For the backend:
```bash
cd backend
npm install
```

For the frontend:
```bash
cd frontend
npm install
```

### 3. Environment Setup

Create a `.env` file in the backend directory:
```env
PORT=5000
MONGODB_URI=mongodb://localhost:27017/blogapp
JWT_SECRET=your_jwt_secret_key_here
NODE_ENV=development
```

### 4. Start MongoDB

Make sure MongoDB is running on your system:
```bash
mongod
```

### 5. Run the application

Start the backend server:
```bash
cd backend
npm start
```

Start the frontend development server:
```bash
cd frontend
npm start
```

The application will be available at `http://localhost:3000`

## 📁 Project Structure

```
blog-app/
├── frontend/                 # React frontend
│   ├── public/
│   ├── src/
│   │   ├── components/       # Reusable UI components
│   │   ├── pages/           # Page components
│   │   ├── services/        # API calls and services
│   │   ├── utils/           # Helper functions
│   │   └── App.js
│   └── package.json
├── backend/                  # Node.js backend
│   ├── controllers/         # Route controllers
│   ├── middleware/          # Custom middleware
│   ├── models/             # MongoDB models
│   ├── routes/             # API routes
│   ├── utils/              # Helper functions
│   ├── server.js           # Main server file
│   └── package.json
└── README.md
```

## 🔧 API Endpoints

### Authentication
- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Login user
- `GET /api/auth/profile` - Get user profile

### Posts
- `GET /api/posts` - Get all posts
- `GET /api/posts/:id` - Get single post
- `POST /api/posts` - Create new post (authenticated)
- `PUT /api/posts/:id` - Update post (authenticated)
- `DELETE /api/posts/:id` - Delete post (authenticated)

### Comments
- `GET /api/posts/:id/comments` - Get post comments
- `POST /api/posts/:id/comments` - Add comment (authenticated)
- `DELETE /api/comments/:id` - Delete comment (authenticated)

## 🎨 UI Components

The frontend uses Material-UI components including:
- Navigation bars and drawers
- Cards for blog posts
- Forms for authentication and post creation
- Buttons, icons, and typography
- Responsive grid system

## 🔐 Authentication Flow

1. User registers/logs in with email and password
2. Server validates credentials and returns JWT token
3. Token is stored in localStorage/sessionStorage
4. Token is sent with authenticated requests in Authorization header
5. Server middleware validates token for protected routes

## 🚦 Available Scripts

### Frontend
- `npm start` - Start development server
- `npm build` - Build for production
- `npm test` - Run tests

### Backend
- `npm start` - Start production server
- `npm run dev` - Start development server with nodemon
- `npm test` - Run tests

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License






## 🙏 Acknowledgments

- React.js team for the amazing framework
- Material-UI for the beautiful components
- Express.js for the robust backend framework
- MongoDB for the flexible database solution

---

**Happy Blogging! 📝✨**
