
Modern Ecommerce Platform

A full-stack ecommerce application built with Next.js, React, TypeScript, Sanity CMS, Clerk Authentication, Stripe Payments, Prisma ORM, Neon PostgreSQL, and Zustand state management.

🚀 Overview

This project is a modern ecommerce platform designed to deliver a fast, scalable, and production-ready shopping experience. It combines a headless CMS architecture with secure authentication, online payments, cloud database infrastructure, and a responsive user interface.

Key Features
Product catalog management
Category-based shopping
Product search and filtering
Shopping cart functionality
Wishlist/Favorites
Secure authentication
Stripe payment processing
Order management
Responsive design
SEO optimization
CMS-powered content management
Admin product management
Customer account dashboard

🏗 System Architecture

┌─────────────────────────┐
│        Customer         │
└────────────┬────────────┘
             │
             ▼
┌─────────────────────────┐
│       Next.js App       │
│   React + TypeScript    │
└───────┬────────┬────────┘
        │        │
        │        │
        ▼        ▼
┌────────────┐ ┌─────────────┐
│   Clerk    │ │  Zustand    │
│ Auth Layer │ │ Cart State  │
└────────────┘ └─────────────┘
        │
        ▼
┌─────────────────────────┐
│     API / Server        │
│   Next.js Route APIs    │
└───────┬────────┬────────┘
        │        │
        ▼        ▼
┌────────────┐ ┌─────────────┐
│  Stripe    │ │   Prisma    │
│  Payments  │ │     ORM     │
└────────────┘ └──────┬──────┘
                      │
                      ▼
              ┌─────────────┐
              │ Neon DB     │
              │ PostgreSQL  │
              └─────────────┘

                      ▲
                      │
              ┌─────────────┐
              │ Sanity CMS  │
              └─────────────┘

🖥 Frontend Layer
Next.js

The application is built using Next.js App Router, providing:

Server-side rendering (SSR)
Static site generation (SSG)
Dynamic routing
API routes
Image optimization
SEO-friendly architecture
Responsibilities
Product pages
Category pages
Checkout experience
Customer dashboard
Search and navigation
React

React powers all interactive user interfaces including:

Product cards
Product galleries
Shopping cart
Checkout forms
Navigation menus
Search components
TypeScript

TypeScript ensures end-to-end type safety across:

Components
API responses
Database models
CMS schemas
Payment flows

Benefits:

Reduced runtime errors
Better maintainability
Improved developer experience
📦 State Management
Zustand

Zustand manages client-side application state.

Cart Store
{
  items: [],
  addItem(),
  removeItem(),
  clearCart()
}
Wishlist Store
{
  favorites: [],
  addFavorite(),
  removeFavorite()
}
UI Store
{
  isCartOpen: false,
  toggleCart()
}

This approach eliminates unnecessary complexity while keeping state management lightweight and performant.

🔐 Authentication
Clerk

Clerk provides complete user authentication and account management.

Features
Email authentication
Google OAuth
GitHub OAuth
Session management
Protected routes
User profiles
Authentication Flow
Visitor
   │
   ▼
Sign Up / Login
   │
   ▼
Clerk Authentication
   │
   ▼
Authenticated User
   │
   ▼
Place Orders
🛍 Content Management
Sanity CMS

Sanity acts as the headless content management system.

Managed Content
Products
Categories
Product Images
Homepage Banners
Promotional Content
SEO Metadata
Benefits
Real-time content updates
Structured content
Scalable architecture
Non-developer friendly management
Example Product Structure
{
  name: "Nike Hoodie",
  slug: "nike-hoodie",
  price: 3999,
  category: "Hoodies",
  images: [],
  description: ""
}
💳 Payments
Stripe

Stripe handles secure payment processing.

Features
Card payments
Checkout sessions
Payment validation
Webhooks
Order confirmation
Checkout Flow
Cart
  │
  ▼
Checkout
  │
  ▼
Stripe Checkout
  │
  ▼
Successful Payment
  │
  ▼
Order Created
🗄 Database Layer
Neon PostgreSQL

Neon provides a serverless PostgreSQL database.

Stores
Users
Orders
Order Items
Payment Records
Customer Activity
Advantages
Serverless scaling
PostgreSQL compatibility
Automatic backups
High performance
Prisma ORM

Prisma serves as the database access layer.

Responsibilities
Database queries
Type-safe operations
Migrations
Relationship management

Example:

const orders = await prisma.order.findMany({
  where: {
    userId
  }
});
📋 Order Processing Flow
Customer Browses Products
          │
          ▼
Products Loaded From Sanity
          │
          ▼
Add Product To Cart
          │
          ▼
Zustand Updates Cart State
          │
          ▼
Proceed To Checkout
          │
          ▼
Authentication Verified By Clerk
          │
          ▼
Stripe Processes Payment
          │
          ▼
Payment Success
          │
          ▼
Order Saved Via Prisma
          │
          ▼
Stored In Neon PostgreSQL
          │
          ▼
Order Visible In User Dashboard
🌟 Technical Highlights
Full TypeScript codebase
Server-side rendering
Headless CMS architecture
Secure authentication
Stripe payment integration
Serverless PostgreSQL database
Modern React state management
SEO optimized pages
Scalable ecommerce architecture
Production-ready deployment
Tech Stack
Technology	Purpose
Next.js	Full-stack Framework
React	UI Development
TypeScript	Type Safety
Zustand	State Management
Clerk	Authentication
Sanity CMS	Content Management
Stripe	Payment Processing
Prisma	ORM
Neon PostgreSQL	Database
Vercel	Deployment



🚀 Projects
🛒 E-Commerce Platform | Laravel + Vue.js + Inertia + Stripe

🔗 Demo: https://youtu.be/7Sop-O-YO8Q
💻 GitHub: https://github.com/RizaldyCondino/Ecommerce
🔗 **[Demo: Ecommerce](https://youtu.be/7Sop-O-YO8Q)**

 ![Image](https://github.com/user-attachments/assets/d72c3c48-c335-48c6-b5bd-c4540f6a350b)
 
💻 **GitHub Repository:** [Ecommerce Project](https://github.com/RizaldyCondino/Ecommerce)

Built a full-stack e-commerce application that supports a complete online shopping experience—from product browsing to checkout.

Key Features:

User authentication and role-based access
Product listing with category and brand filtering
Dynamic search with debounce
Shopping cart and cart management system
Order processing workflow
Stripe payment integration (test mode)
Responsive UI using Vue.js and Flowbite

What I handled:

Designed backend architecture using Laravel
Built and managed database relationships (products, orders, users)
Implemented cart logic and checkout flow
Integrated Stripe API for secure payments
Developed interactive frontend using Vue + Inertia

This project demonstrates real-world full-stack development, including backend logic, frontend interaction, and third-party integration.

⚠️ Payment integration is currently in progress.
The checkout flow and order creation are implemented, but live payment confirmation and stock updates after payment are still being finalized.

---

📦 Employee Management System
📌 Status: 🟡 In Progress (Not yet completed)

This project is currently under development and will continue to be improved with additional features and refinements.
A full-featured Employee Management System designed to handle core HR operations such as employee records, departments, leave requests, payroll, attendance tracking, and company announcements.
- Built with **Laravel + MySQL**
- 📌 Focus: Backend logic & database relationships
🚀 Project Preview
 <img width="1917" height="951" alt="Image" src="https://github.com/user-attachments/assets/7f297e1b-a34a-44bc-b8c2-9bd172142f39" />

💻 <b>GitHub Repository:</b> 
<a href="https://github.com/RizaldyCondino/-Employee-Management-System/tree/main">Employee Management System</a>


- 🚀 Features
- 👨‍💼 Employee Management  
- 🏢 Department Management  
- 📝 Leave Management System (Request & Approval Workflow)  
- 💰 Payroll Management System  
- 📊 Attendance Tracking System  
- 📢 Company Announcements  

🛠️ Tech Stack
- 🧩 Laravel (Backend Framework)  
- ⚛️ React.js (Frontend)  
- 🗄️ MySQL (Database)  
- 🔗 Inertia.js (SPA-style bridge)  

---

📦 Listing App (Laravel + Vue)

A full-stack listing management system built using Laravel 11, Vue.js, and Inertia.js.
This application allows users to manage products, categories, and brands with role-based access for both admin and regular users.

🎥 <b>Actual Tutorial Used:</b>
<a href="https://www.youtube.com/watch?v=NZUspvmsNfw&list=PL38wFHH4qYZUdIKP9jG371N3G4kbWAg2c" target="_blank">
Listing App Project
</a>

By: Learn with Jon

🚀 Project Preview
<p align="center"> <img src="https://github.com/user-attachments/assets/04bf28a8-4b2a-42b9-9ac6-d8d85adbe4c0" width="100%" /> </p>
💻 <b>GitHub Repository:</b> 
<a href="https://github.com/RizaldyCondino/ListingApp">Listing App</a>

🎯 What I Learned
Through this project, 

I learned how to:

Build a full-stack web application using modern tools
Manage database relationships effectively
Implement authentication and role-based access control
Design interactive and responsive UI components
Work with Laravel + Vue.js integration using Inertia.js
