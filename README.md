# 🌾 SMART-AGRICONNECT

![Smart AgriConnect Banner](https://placehold.co/1200x400/2d5e3d/white?text=SMART-AGRICONNECT+Banner)

A unified digital platform designed to empower farmers through technology, providing tools for subsidy navigation, crop recommendations, digital marketplaces, farm management, and community engagement.

## 📌 Table of Contents
- [Problem Statement](#-problem-statement)
- [Solution](#-solution)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)
- [Installation](#-installation)
- [Environment Variables](#-environment-variables)
- [Key Features](#-key-features)
- [Screenshots](#-screenshots)
- [API Endpoints](#-api-endpoints)
- [License](#-license)

## 🌾 Problem Statement

| Challenge                  | Impact                             |
|----------------------------|------------------------------------|
| Unclear subsidy information | Farmers miss financial benefits    |
| No crop demand data        | Oversupply leading to low prices   |
| Fragmented knowledge sharing | Limited access to expert advice  |
| Manual trading processes   | Inefficient market access          |
| Outdated farm practices    | Reduced productivity               |

## 💡 Solution
**Five Integrated Modules:**
1. **Subsidy Navigator** - Real-time government scheme tracking
2. **Crop Oracle** - AI-powered planting recommendations
3. **AgriMarket** - Digital trading with escrow
4. **Farm Genius** - IoT-ready management system
5. **Krishi Community** - Verified expert Q&A platform

## 🛠 Tech Stack

### Frontend
- **React 18+**: Component-based UI
- **Vite**: Fast build tool
- **Tailwind CSS**: Utility-first styling
- **Axios**: HTTP requests
- **React Router**: Navigation

### Backend
- **Node.js 16+**: Runtime environment
- **Express**: Web framework
- **Mongoose**: MongoDB ORM
- **JWT**: Authentication
- **Cloudinary**: Media storage

### DevOps
- **Docker**: Containerization
- **GitHub Actions**: CI/CD pipelines
- **ESLint**: Code quality
- **Prettier**: Code formatting

## 📂 Project Structure
SMART-AGRICONNECT/
├── admin/
│ ├── node_modules/
│ ├── public/
│ │ ├── assets/
│ │ └── index.html
│ ├── src/
│ │ ├── components/
│ │ ├── pages/
│ │ ├── App.jsx
│ │ └── main.jsx
│ ├── .dockerignore
│ ├── Dockerfile
│ ├── package.json
│ └── vite.config.js
├── backend/
│ ├── config/
│ │ └── db.js
│ ├── controllers/
│ │ ├── authController.js
│ │ └── subsidyController.js
│ ├── models/
│ │ ├── User.js
│ │ └── Subsidy.js
│ ├── routes/
│ │ ├── authRoutes.js
│ │ └── apiRoutes.js
│ ├── utils/
│ │ ├── cloudinary.js
│ │ └── jwt.js
│ ├── .env
│ ├── package.json
│ └── server.js
├── user/
│ ├── node_modules/
│ ├── public/
│ │ └── index.html
│ ├── src/
│ │ ├── components/
│ │ ├── pages/
│ │ ├── App.jsx
│ │ └── main.jsx
│ ├── package.json
│ └── vite.config.js


## 🚀 Installation

### Prerequisites
- **Node.js v16+**
- **MongoDB 5.0+**
- **Git**

### Setup Instructions
1. **Clone the repository**
   ```bash
   git clone https://github.com/SUKANT43/Smart-AgriConnect.git
   cd Smart-AgriConnect
Backend Setup

bash
cd backend
npm install
cp .env.example .env  # Update with your credentials
npm start
Frontend (User Portal) Setup

bash
cd ../user
npm install
npm run dev
Admin Panel Setup

bash
cd ../admin
npm install
npm run dev
Running with Docker

bash
docker-compose up --build
🌍 Environment Variables
Create a .env file in the /backend directory with the following content:

env
PORT=5000
MONGO_URI=mongodb://localhost:27017/smartagri
JWT_SECRET=your_secure_secret
JWT_EXPIRE=30d
CLOUDINARY_NAME=your_cloud_name
CLOUDINARY_KEY=your_api_key
CLOUDINARY_SECRET=your_api_secret
✨ Key Features
Admin Portal

User management dashboard

Analytics and reporting

Content moderation tools

System configuration panel

Farmer Dashboard

Subsidy Navigator: Real-time government scheme tracking

Crop Advisor: Data-driven planting recommendations

Marketplace: Digital trading platform

Farm Manager: Production tracking tools

Community Hub: Discussion forums

API Services

RESTful endpoints with JWT authentication

Role-based access control

Rate limiting and request validation

Swagger documentation

Database

MongoDB Atlas cloud integration

Optimized schemas for agricultural data

Indexed queries for performance

Regular backup system

📸 Screenshots
<div align="center"> <img src="https://placehold.co/600x400?text=Admin+Dashboard" alt="Admin Dashboard" width="30%"> <img src="https://placehold.co/600x400?text=Farmer+Portal" alt="Farmer Portal" width="30%"> <img src="https://placehold.co/600x400?text=Mobile+View" alt="Mobile View" width="30%"> </div>
🔌 API Endpoints
🛡️ Authentication
Endpoint	Method	Description
/api/auth/register	POST	Register new user
/api/auth/login	POST	User login
/api/auth/me	GET	Get current user
💰 Subsidies
Endpoint	Method	Description
/api/subsidies	GET	List all subsidies
/api/subsidies/:id	GET	Get subsidy details
/api/subsidies/apply	POST	Apply for subsidy
🛒 Marketplace
Endpoint	Method	Description
/api/market/listings	GET	Get all listings
/api/market/listings	POST	Create new listing
/api/market/listings/:id	GET	Get listing details
👥 Community
Endpoint	Method	Description
/api/community/posts	GET	Get all posts
/api/community/posts	POST	Create new post
/api/community/posts/:id	GET	Get post details
📜 License
This project is licensed under the MIT License - see the LICENSE file for details.


This consolidated markdown file:
1. Maintains proper section ordering
2. Preserves all original content
3. Fixes formatting issues
4. Ensures consistent heading levels
5. Properly organizes code blocks and tables
6. Maintains all links and images
