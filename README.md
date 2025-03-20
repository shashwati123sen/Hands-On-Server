# HandsOn - Backend

## 📌 Project Overview
HandsOn is a community-driven social volunteering platform. This repository contains the **Node.js backend**, which provides API endpoints for:

- Event creation, listing, and filtering
- One-click event registration
- Community help request posting and response
- User authentication and data management

## 🛠️ Tech Stack
- **Backend**: Node.js (Express.js)
- **Database**: MongoDB (Mongoose for ODM)
- **Authentication**: JWT-based authentication
- **API Communication**: REST API

## 📂 Project Structure
```
backend/
│── src/
│   ├── controllers/   # Business logic for routes
│   ├── models/        # Mongoose models (Event, User, etc.)
│   ├── routes/        # API endpoints
│   ├── middlewares/   # Authentication & validation middleware
│   ├── config/        # Database connection & environment variables
│   ├── server.js      # Main server file
│── .env               # Environment variables
│── package.json
│── README.md
```

## 🔧 Setup & Installation

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/yourusername/hands-on-backend.git
cd hands-on-backend
```

### 2️⃣ Install Dependencies
```bash
npm install  # or yarn install
```

### 3️⃣ Set Up Environment Variables
Create a `.env` file in the root directory:
```env
PORT=5000
MONGO_URI=mongodb+srv://your_mongodb_url
JWT_SECRET=your_jwt_secret
```

### 4️⃣ Run the Server
```bash
npm start  # or nodemon src/server.js
```
The backend will be available at `http://localhost:5000/`.

## 🚀 API Endpoints
### User Authentication
- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Authenticate user & return token

### Event Management
- `POST /api/events` - Create a new event
- `GET /api/events` - Get all events (with filters)
- `POST /api/events/:id/register` - Register for an event

### Community Help Requests
- `POST /api/help` - Create a new help request
- `GET /api/help` - List all help requests
- `POST /api/help/:id/respond` - Respond to a help request

## 📝 Contribution Guidelines
1. **Fork** the repository.
2. Create a **feature branch** (`feature/your-feature-name`).
3. **Commit** your changes (`git commit -m 'Add new feature'`).
4. **Push** to the branch (`git push origin feature/your-feature-name`).
5. Submit a **Pull Request**.

## 📜 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

🎯 **Happy Coding & Volunteering!** 🚀
