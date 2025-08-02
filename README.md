# 🍽️ Canteen Ease - Food Delivery Platform

A full-stack food delivery application built with React, Node.js, and MongoDB. This project includes a customer-facing frontend, admin panel, and backend API.

## 📋 Table of Contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)
- [License](#license)

## ✨ Features

### Customer Features
- 🍕 Browse and search food items
- 🛒 Add items to cart with quantity management
- 💳 Secure payment integration with Stripe
- 📱 Responsive design for mobile and desktop
- 👤 User authentication and profile management
- 📦 Order tracking and history
- ⭐ Real-time order status updates

### Admin Features
- 📊 Dashboard with order management
- 🍽️ Add, edit, and delete food items
- 📸 Image upload for food items
- 📈 View order statistics
- 👥 Manage user accounts
- 📋 Process and update order status

## 🛠️ Tech Stack

### Frontend
- **React 18** - UI framework
- **Vite** - Build tool and dev server
- **React Router DOM** - Client-side routing
- **Axios** - HTTP client
- **React Toastify** - Notifications
- **Stripe.js** - Payment processing

### Backend
- **Node.js** - Runtime environment
- **Express.js** - Web framework
- **MongoDB** - Database
- **Mongoose** - ODM for MongoDB
- **JWT** - Authentication
- **Multer** - File upload handling
- **Stripe** - Payment gateway
- **bcrypt** - Password hashing
- **CORS** - Cross-origin resource sharing

## 📁 Project Structure

```
food-del/
├── frontend/          # Customer-facing React app
│   ├── src/
│   │   ├── components/    # Reusable UI components
│   │   ├── pages/         # Page components
│   │   ├── Context/       # React context for state management
│   │   └── assets/        # Images and static files
│   └── package.json
├── admin/             # Admin panel React app
│   ├── src/
│   │   ├── components/    # Admin UI components
│   │   ├── pages/         # Admin pages
│   │   └── assets/        # Admin assets
│   └── package.json
├── backend/           # Node.js API server
│   ├── config/        # Database configuration
│   ├── controllers/   # Route controllers
│   ├── middleware/    # Custom middleware
│   ├── models/        # MongoDB schemas
│   ├── routes/        # API routes
│   ├── uploads/       # File uploads
│   └── server.js      # Main server file
└── README.md
```

## 🚀 Installation

### Prerequisites
- Node.js (v16 or higher)
- MongoDB
- Git

### Backend Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/Prathima0208/Canteen_ease.git
   cd Canteen_ease/food-del
   ```

2. **Install backend dependencies**
   ```bash
   cd backend
   npm install
   ```

3. **Environment Setup**
   Create a `.env` file in the backend directory:
   ```env
   PORT=4000
   MONGODB_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   STRIPE_SECRET_KEY=your_stripe_secret_key
   ```

4. **Start the backend server**
   ```bash
   npm run server
   ```

### Frontend Setup

1. **Install frontend dependencies**
   ```bash
   cd ../frontend
   npm install
   ```

2. **Start the frontend development server**
   ```bash
   npm run dev
   ```

### Admin Panel Setup

1. **Install admin dependencies**
   ```bash
   cd ../admin
   npm install
   ```

2. **Start the admin panel**
   ```bash
   npm run dev
   ```

## 📖 Usage

### Running the Application

1. **Start all services**
   ```bash
   # Terminal 1 - Backend
   cd backend && npm run server
   
   # Terminal 2 - Frontend
   cd frontend && npm run dev
   
   # Terminal 3 - Admin Panel
   cd admin && npm run dev
   ```

2. **Access the applications**
   - Frontend: http://localhost:5173
   - Admin Panel: http://localhost:5174
   - Backend API: http://localhost:4000

### Default Admin Credentials
- Email: admin@canteenease.com
- Password: admin123

## 🔌 API Endpoints

### Authentication
- `POST /api/user/register` - User registration
- `POST /api/user/login` - User login
- `GET /api/user/profile` - Get user profile

### Food Items
- `GET /api/food` - Get all food items
- `POST /api/food` - Add new food item (admin only)
- `PUT /api/food/:id` - Update food item (admin only)
- `DELETE /api/food/:id` - Delete food item (admin only)

### Cart
- `GET /api/cart` - Get user cart
- `POST /api/cart` - Add item to cart
- `DELETE /api/cart/:id` - Remove item from cart

### Orders
- `POST /api/order` - Create new order
- `GET /api/order` - Get user orders
- `GET /api/order/all` - Get all orders (admin only)
- `PUT /api/order/:id` - Update order status (admin only)

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Prathima** - [GitHub Profile](https://github.com/Prathima0208)

## 🙏 Acknowledgments

- React team for the amazing framework
- Vite for the fast build tool
- MongoDB for the database
- Stripe for payment processing
- All contributors and supporters

---

⭐ If you found this project helpful, please give it a star on GitHub! 