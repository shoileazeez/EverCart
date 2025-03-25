# EverCart - E-commerce Platform

EverCart is a full-featured e-commerce platform built with React.js (frontend) and Django REST Framework (backend). The project follows a structured development workflow using feature branches and separate deployment branches for frontend and backend.

---

## **Development Workflow**

### **Branching Strategy**
- **Frontend Development:** Features should be developed in `feature/frontend-[feature-name]` branches and merged into the `frontend` branch after review.
- **Backend Development:** Features should be developed in `feature/backend-[feature-name]` branches and merged into the `backend` branch after review.
- **Deployment:** The `frontend` branch is used for deploying the frontend, while the `backend` branch is used for deploying the backend.

---

## **API Endpoints (Example)**

### **Authentication**
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `GET /api/auth/user` - Get user details
- `POST /api/auth/google` - Google authentication

### **Products**
- `GET /api/products` - Get all products
- `GET /api/products/:id` - Get single product details

### **Cart & Orders**
- `POST /api/cart/add` - Add item to cart
- `GET /api/cart` - View cart
- `POST /api/order/checkout` - Checkout and place order

### **Payments**
- `POST /api/payment/paystack` - Pay using Paystack (local payments)
- `POST /api/payment/stripe` - Pay using Stripe (USD payments)
- `POST /api/payment/chapa` - Pay using Chapa (Ethiopian payment gateway)

---

## **API Documentation**
You can find the API documentation here: **https://app.getpostman.com/join-team?invite_code=de1783e195de95e893621d61f9b31bfdfdac6fc630e1e73ccde8eb1160bfdc19&target_code=dcc9268d8a36e6c66a54cb2d0e9d3d04**

---

## **Tech Stack**

### **Frontend:**
- React.js (with Vite for fast development)
- Tailwind CSS for styling
- Axios for API requests

### **Backend:**
- Django (Django REST Framework for API)
- PostgreSQL for the database
- JWT authentication for security
- Django Toolkit for Google Authentication

### **Tools & Services:**
- Postman for API documentation and testing
- Paystack for local payments
- Stripe for international (USD) payments
- Chapa for Ethiopian payment gateway

---

## **Features**

### **Frontend:**
- User-friendly UI/UX
- Product browsing and search functionality
- Shopping cart management
- Secure user authentication and profile management
- Responsive design for mobile and desktop

### **Backend:**
- RESTful API for frontend communication
- Secure authentication and authorization
- Google authentication using Django Toolkit
- Product and order management
- Payment gateway integration (Paystack, Stripe, Chapa)
- Admin dashboard for managing users and orders

---

## **Git Workflow Commands**

### **Cloning the Repository**
```sh
git clone https://github.com/shoileazeez/EverCart.git
cd evercart
```

### **Updating the Repository**
```sh
git pull origin main  # Get the latest changes
```

### **Creating a Feature Branch**
```sh
# For frontend feature
git checkout -b feature/frontend-[feature-name]

# For backend feature
git checkout -b feature/backend-[feature-name]
```

### **Merging Features into Deployment Branches**
```sh
# Merge frontend features into the frontend branch
git checkout frontend
git merge feature/frontend-[feature-name]
git push origin frontend

# Merge backend features into the backend branch
git checkout backend
git merge feature/backend-[feature-name]
git push origin backend
```

---

## **Deployment Instructions**

### **Backend Deployment (`backend` branch)**
```sh
git checkout backend
git pull origin backend
```

### **Frontend Deployment (`frontend` branch)**
```sh
git checkout frontend
git pull origin frontend
```

---

## **Contributors**
Feel free to contribute to EverCart by submitting pull requests! 🚀


