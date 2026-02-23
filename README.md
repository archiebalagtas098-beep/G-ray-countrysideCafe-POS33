☕ G-ray Countryside Cafe POS33
A Point of Sale (POS) system designed for G-ray Countryside Cafe, built using Node.js, Express, MongoDB, and real-time WebSocket communication.
This system handles authentication, orders, transactions, email notifications, and live updates.
📦 Dependencies Used
This project uses only the following dependencies:
Production Dependencies
bcryptjs – Password hashing
catch-express – Express error handling utility
cookie-parser – Parse cookies from HTTP requests
dotenv – Environment variable management
ejs – Server-side templating engine
express – Web framework for Node.js
jsonwebtoken – JWT authentication
mongoose – MongoDB object modeling
nodemailer – Email sending service
ws – WebSocket support for real-time features
Development Dependency
nodemon – Auto-restart server during development
📁 Project Structure (Suggested)
Copy code

G-ray-countrysideCafe-POS33/
│
├── controllers/        # Request logic
├── models/             # Mongoose schemas
├── routes/             # Express routes
├── views/              # EJS templates
├── public/             # Static assets (CSS, JS)
├── middlewares/        # Auth & error handling
├── config/             # Database & environment config
│
├── .env                # Environment variables
├── app.js              # Express app setup
├── server.js           # Server entry point
├── package.json
└── README.md
⚙️ Environment Variables
Create a .env file in the root directory:
Copy code

PORT=3000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
EMAIL_USER=your_email
EMAIL_PASS=your_email_password
🚀 Installation & Setup
1️⃣ Clone the Repository
Copy code

git clone https://github.com/your-username/G-ray-countrysideCafe-POS33.git
cd G-ray-countrysideCafe-POS33
2️⃣ Install Dependencies
Copy code

npm install
3️⃣ Run the Application
Development mode
Copy code

npm run dev
Production mode
Copy code

npm start
🔐 Authentication
Passwords are securely hashed using bcryptjs
User sessions are managed with JWT
Cookies are handled using cookie-parser
📡 Real-Time Features
Uses WebSockets (ws) for:
Live order updates
POS synchronization
Real-time notifications
📧 Email Notifications
nodemailer is used for:
Order confirmations
Admin alerts
System notifications
🖥️ View Engine
EJS is used for rendering dynamic pages such as:
Login
Dashboard
Orders
POS interface
🛠 Error Handling
Centralized error handling powered by catch-express
Clean API error responses
🧪 Development Tools
nodemon automatically restarts the server on file changes
📌 Requirements
Node.js v16+
MongoDB (local or cloud)
📄 License
This project is intended for educational and internal cafe use.
All rights reserved © G-ray Countryside Cafe.
