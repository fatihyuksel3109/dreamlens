# DreamLens

## Overview
DreamLens is a React Native application that allows users to submit their dreams and receive AI-generated interpretations using OpenAI's API. User data and dream histories are stored in a MongoDB database through a Node.js and Express backend.

## Tech Stack
### **Frontend:**
- React Native (Expo)
- Zustand / Redux (State Management)
- React Native Paper (UI Components)
- i18next (Multilingual Support)

### **Backend:**
- Node.js with Express.js
- MongoDB with Mongoose
- OpenAI API (GPT-4 for dream interpretation)
- Firebase Auth (Authentication)

### **Hosting & Deployment:**
- Expo EAS for mobile app
- Vercel (Frontend Hosting)
- Render/Fly.io (Backend Hosting)

## Features
- Submit dreams and receive AI-generated interpretations
- User authentication via Firebase or JWT
- Dark mode support
- Multilingual support (Turkish, English, French, Spanish, German, Arabic) using i18next
- Save dream history in MongoDB
- Share dream interpretations with others

## App Screens & Flow
### **1. Onboarding Process:**
- Welcome Screen with App Introduction
- Language Selection Screen
- Sign Up / Login Screen (Firebase Auth or JWT)

### **2. Main Screens:**
- **Home Screen:** Submit a dream for interpretation
- **Dream Interpretation Screen:** View AI-generated response
- **History Screen:** List of past dream interpretations
- **Profile Screen:** Manage user profile and settings

### **3. Additional Features:**
- Dark Mode Toggle
- Multilingual Selection
- Share Interpretation with Others
- Delete or Edit Dream History Entry

## Installation & Setup
### **1. Clone the Repository**
```sh
 git clone https://github.com/fatihyuksel3109/dreamlens.git
 cd dreamlens
```

### **2. Install Dependencies**
```sh
 npm install
```

### **3. Configure Environment Variables**
Create a `.env` file in the root directory and add:
```
MONGO_URI=your_mongodb_connection_string
OPENAI_API_KEY=your_openai_api_key
JWT_SECRET=your_jwt_secret_key
```

### **4. Start the Backend Server**
```sh
 cd backend
 npm install
 npm start
```

### **5. Start the Expo App**
```sh
 cd frontend
 npm start
```

## API Endpoints
| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/dreams` | Submit a dream and receive an interpretation |
| GET | `/api/dreams` | Fetch user dream history |
| POST | `/api/auth/signup` | Register a new user |
| POST | `/api/auth/login` | Authenticate a user |

## Future Enhancements
- Implement AI-driven personalized dream analysis
- Support for voice input and AI-powered voice responses
- Cloud-based storage for dream history and profiles

## Contributing
1. Fork the repository
2. Create a feature branch (`git checkout -b feature-name`)
3. Commit your changes (`git commit -m 'Add new feature'`)
4. Push to the branch (`git push origin feature-name`)
5. Open a pull request

## License
This project is licensed under the MIT License.

