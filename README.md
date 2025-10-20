# 🍴 Restaurant Food Ordering App (Node.js + Express + MongoDB)

A complete **Restaurant Food Ordering Backend API** built using **Node.js**, **Express**, and **MongoDB**.  
It provides secure authentication, restaurant and food management, order processing, and category-based filtering.

This project demonstrates strong backend skills, REST API design, role-based authentication, and database modeling using Mongoose.

---

## 🚀 Features

### 👨‍🍳 For Customers
- Register and login securely with JWT authentication
- Browse all restaurants and food items
- Filter food by category or restaurant
- Place and view orders

### 🏪 For Restaurant Owners / Admin
- Create and manage restaurant profiles
- Add, edit, and delete food items
- Categorize dishes (e.g., Veg, Non-Veg, Beverages)
- Manage incoming customer orders
- Role-based access control using middleware

---

## 🧱 Tech Stack

| Layer | Technology |
|--------|-------------|
| **Backend Framework** | Node.js + Express.js |
| **Database** | MongoDB with Mongoose |
| **Authentication** | JWT + bcrypt.js |
| **Middlewares** | Express middleware, Auth, Admin |
| **Environment Config** | dotenv |
| **API Testing** | Postman / Thunder Client |

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the repository
```bash
git clone https://github.com/YOUR-USERNAME/nodejs-resturant-food-app.git
cd nodejs-resturant-food-app
```

### 2️⃣ Install dependencies
```bash
npm install
```

### 3️⃣ Configure environment variables
Create a `.env` file in the root directory:
```
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
```

### 4️⃣ Start the server
```bash
npm run dev
```
Server runs on → **http://localhost:5000**

---

## 📘 API Endpoints Overview

| Method | Endpoint | Description |
|--------|-----------|-------------|
| `POST` | `/api/auth/register` | Register a new user |
| `POST` | `/api/auth/login` | Login user and return JWT token |
| `GET` | `/api/resturant` | Get all restaurants |
| `POST` | `/api/resturant` | Add new restaurant (admin only) |
| `GET` | `/api/food` | Get all food items |
| `POST` | `/api/food` | Add food item (restaurant owner) |
| `GET` | `/api/category` | Get all food categories |
| `POST` | `/api/category` | Create a new category |
| `GET` | `/api/user/orders` | Get logged-in user orders |
| `POST` | `/api/order` | Place a new order |

---

## 🗂️ Folder Structure

```
nodejs-resturant-food-app/
├── config/
│   └── db.js
├── controllers/
│   ├── authControllers.js
│   ├── categoryController.js
│   ├── foodController.js
│   ├── resturantController.js
│   └── userController.js
├── middlewares/
│   ├── adminMiddleware.js
│   └── authMiddleware.js
├── models/
│   ├── categoryModel.js
│   ├── foodModal.js
│   ├── orderModel.js
│   ├── resturantModel.js
│   └── userModel.js
├── routes/
│   ├── authRoutes.js
│   ├── catgeoryRoutes.js
│   ├── foodRoutes.js
│   ├── resturantRoutes.js
│   └── userRoutes.js
├── data.js
├── server.js
└── package.json
```

---

## 🔐 Security & Middleware
- JWT-based authentication for users and admins  
- Role-based route protection using custom middlewares  
- Error handling for invalid or unauthorized access  
- Environment variables hidden via `.env`

---

## 🧠 Learning Outcomes
- Designed RESTful APIs using Express.js  
- Used MongoDB with Mongoose for data modeling  
- Implemented JWT authentication & role-based access  
- Followed MVC architecture for clean code separation  
- Practiced modular Node.js structure and route handling

---

## 🧾 Future Enhancements
- Payment gateway integration (Stripe / Razorpay)  
- Admin dashboard analytics (Top orders, revenue)  
- Image upload support using Multer  
- Real-time order status tracking (Socket.io)

---

## 👨‍💻 Author
**Your Name**  
Backend Developer | Node.js | MongoDB | Express  
📧 sreeharirpillai2002@gmail.com 
🔗https://github.com/sreehari-r-pillai 

---

### 🏁 Project Status: `Completed ✅`
This project serves as a backend demonstration of real-world REST API design and can be extended for full-stack (React/Next.js) applications.
