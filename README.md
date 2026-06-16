# e-commerce-epi
online trade and market
# 🛒 E-Shop: Full-Stack E-Commerce Platform

> A production-ready, full-stack e-commerce application featuring a dynamic product catalog, secure multi-step checkout, and an integrated admin dashboard.

## 🔗 Live Links & Previews
* **Live Storefront:** [View Live Demo](https://vercel.app)
* **Backend API Docs:** [View Swagger API Specs](https://render.com)

---

## ✨ Core Features
* **User Authentication:** Secure signup, login, and session persistence using JWT and HTTP-only cookies.
* **Product Catalog:** Advanced filtering, category sorting, search functionality, and real-time stock inventory tracking.
* **Shopping Cart & Checkout:** Persistent shopping cart state with integrated **Stripe Payment Gateway** for secure credit card processing.
* **Admin Dashboard:** Role-based access control allowing admins to create, update, or delete products and manage customer order fulfillment statuses.
* **Responsive UI:** Fully optimized user interface across mobile, tablet, and desktop devices.

---

## 🛠️ Tech Stack
* **Frontend:** React.js, Redux Toolkit (State Management), Tailwind CSS, Axios
* **Backend:** Node.js, Express.js, JSON Web Tokens (JWT)
* **Database:** MongoDB & Mongoose (Object Data Modeling)
* **Payments:** Stripe API

---

## ⚙️ Local Installation Guide

Follow these steps to set up the development environment on your computer:

### 1. Clone the Project
```bash
git clone https://github.com
cd your-ecommerce-repo
```

### 2. Install Dependencies
```bash
# Install root, backend, and frontend packages
npm run install-all
```

### 3. Set Up Environment Variables
Create a `.env` file in the root backend directory:
```env
PORT=5000
MONGO_URI=mongodb+srv://your_username:your_password@cluster.mongodb.net/eshop
JWT_SECRET=your_jwt_signing_secret_key
STRIPE_SECRET_KEY=sk_test_your_stripe_private_key
```

### 4. Seed Database & Run
```bash
# Optional: Seed the database with sample products
npm run seed-data

# Start both the frontend and backend servers concurrently
npm run dev
```

---

## 🗄️ Database Architecture
The platform relies on three highly structured data models to manage business logic:
* **User Schema:** Tracks profile information, encrypted passwords, and roles (`customer` or `admin`).
* **Product Schema:** Stores names, images, descriptions, categories, pricing, and exact `countInStock` metrics.
* **Order Schema:** Links buyers to purchased items, logs delivery addresses, and records Stripe `isPaid` confirmations.

---

## 📝 License
Distributed under the MIT License. See `LICENSE` for more details.
