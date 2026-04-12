# E-Commerce Platform
A full-stack MERN e-commerce app with a customer storefront, admin panel, and Express REST API. Features Stripe Checkout, JWT auth, and Cloudinary image uploads.

## Features
- JWT authentication with bcrypt password hashing
- Product catalogue with category/subcategory filtering and search
- Persistent cart sync across sessions
- Stripe Checkout with server-side session verification
- Admin panel for product management and order status tracking
- Cloudinary image uploads

## Tech Stack
- Frontend: React 19, Vite, Tailwind CSS v4, React Router DOM v7, Axios
- Admin Panel: React 19, Vite, Tailwind CSS v4, Axios
- Backend: Node.js, Express 5, Mongoose, JWT, bcrypt, Multer
- Database: MongoDB Atlas
- Payments: Stripe Checkout
- Image Storage: Cloudinary
- Deployment: Vercel

## Project Structure
```
e-commerce/
├── frontend/   # Customer storefront (React + Vite)
├── admin/      # Admin panel (React + Vite)
├── backend/    # REST API (Express + MongoDB)
└── README.md
```

## Getting Started
**Prerequisites**: Node.js, MongoDB Atlas, Cloudinary, Stripe account

Open 3 terminals from the project root:
```
cd frontend && npm run dev
cd backend && npm run server
cd admin && npm run dev
```

Frontend and Admin run on Vite dev servers. Backend runs on `http://localhost:4000`.

### Environment Variables

Backend (.env):
```
MONGODB_URI=your_mongodb_uri
CLOUDINARY_NAME=your_name
CLOUDINARY_API_KEY=your_key
CLOUDINARY_SECRET_KEY=your_secret
JWT_SECRET=your_secret
ADMIN_EMAIL=your_email
ADMIN_PASSWORD=your_password
STRIPE_SECRET_KEY=sk_test_...
```

Frontend (.env):
```
VITE_BACKEND_URL=http://localhost:4000
```
