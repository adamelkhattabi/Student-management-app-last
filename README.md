# Student Management App - Frontend

A React-based student management system with Firebase authentication and a RESTful API backend.

## 🚀 Features

- User authentication (Login/Register) with Firebase
- Student CRUD operations (Create, Read, Update, Delete)
- Protected routes for authenticated users
- Responsive design with custom CSS
- Real-time authentication state management

## 📋 Prerequisites

Before you begin, ensure you have the following installed:

- **Node.js** (v14 or higher) - [Download](https://nodejs.org/)
- **npm** (v6 or higher) - comes with Node.js
- **Git** - [Download](https://git-scm.com/)
- **Backend server** - Running on port 5000 (see backend setup below)

## 🛠️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/adamelkhattabi/Student-management-app-last.git
cd Student-management-app-last

Install dependencies
bash
npm install

 Set up environment variables
Create a .env file in the root directory:

bash
touch .env

 Set up environment variables
Create a .env file in the root directory:

bash
touch .env

PORT=5000
MONGODB_URI=      ( replace with your mongodb uri)

Configure Firebase
Create a src/firebase.js with your firebaseconfig code


5. Set up Firebase Project
Go to Firebase Console

Click "Create a project" or select an existing one

Add a web app to your project (click </> icon)

Copy the firebaseConfig object values

Enable Authentication:

Go to "Authentication" → "Sign-in methods"

Enable "Email/Password" authentication

Create a test user (Authentication → Add user)

6. Start the Backend Server
Make sure your backend server is running on port 5000:

bash
cd ../backend  # Navigate to backend directory
npm install
npm start

7. Start the Frontend Application
bash
cd ../frontend  # Navigate back to frontend
npm start


Project Structure
text
frontend/
├── public/
│   ├── index.html
│   └── ...
├── src/
│   ├── components/
│   │   ├── Login.js
│   │   └── StudentList.js
│   ├── App.js
│   ├── App.css
│   ├── firebase.js
│   ├── api.js
│   └── index.js
├── .env
├── .gitignore
├── package.json
└── README.md
🔧 Available Scripts
Command	Description
npm start	Runs the app in development mode
npm build	Builds the app for production
npm test	Launches the test runner
npm eject	Ejects from create-react-app


🚦 Usage
Login/Register
First-time users can register with email and password

Existing users can log in with their credentials

Firebase handles all authentication securely

Managing Students
After logging in, you can:

View all students in a table

Add new students with name, email, grade, age, and address

Edit existing student information

Delete students from the system

Logout
Click the "Logout" button in the header to end your session
