# postaway
📱 Social Media API
A RESTful backend API for a social media platform built using Node.js, Express, and MongoDB (Mongoose). This project supports user authentication, posts, comments, likes, and profile management.

🚀 Features


🔐 User Authentication (Register/Login)


👤 User Profile Management


📝 Create, Read, Update, Delete Posts


💬 Comment on Posts


❤️ Like/Unlike Posts


📂 File Upload Support (Profile/Post Images)


🛡️ Middleware-based Authentication & Error Handling


📜 Logging System



🛠️ Tech Stack


Node.js


Express.js


MongoDB (Mongoose)


JWT Authentication


Multer (for file uploads)



📁 Project Structure
social-media-api/│├── controllers/│   ├── userController.js│   ├── postController.js│   ├── commentController.js│   ├── likeController.js│   └── userProfileController.js│├── models/│   ├── userModel.js│   ├── postModel.js│   └── commentModel.js│├── middlewares/│   ├── authMiddleware.js│   ├── errorMiddleware.js│   ├── logger.js│   └── uploadMiddleware.js│├── app.js├── package.json└── .env

⚙️ Installation


Clone the repository:


git clone <your-repo-link>cd social-media-api


Install dependencies:


npm install


Create a .env file:


PORT=5000MONGO_URI=your_mongodb_connection_stringJWT_SECRET=your_secret_key


Start the server:


npm start

📌 API Endpoints (Sample)
🔑 Auth


POST /api/users/register


POST /api/users/login


👤 User


GET /api/users/profile


PUT /api/users/profile


📝 Posts


POST /api/posts


GET /api/posts


DELETE /api/posts/:id


💬 Comments


POST /api/comments/:postId


DELETE /api/comments/:id


❤️ Likes


POST /api/likes/:postId



🔒 Authentication


Uses JWT (JSON Web Tokens)


Protected routes require token in headers:


Authorization: Bearer <token>

📷 File Upload


Uses Multer


Supports image upload for:


Profile pictures


Posts





🧪 Testing
You can test APIs using:


Postman


Thunder Client



🧑‍💻 Author


Developed as part of a backend learning project


