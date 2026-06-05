<h2>👨‍💻 About Me</h2>
      <p>
       I'm an aspiring Junior FullStack who enjoys building modern, responsive, and functional web applications. I like turning ideas into clean and user-friendly interfaces while continuously learning and improving my skills as a developer.
      </p>
      <p>
        🚀 Goal: Become a Junior Fullstack developer <br/>
        💡 Currently working on: E-commerce projects <br/>
        📍 Based in: Philippines
      </p>

## 🌐 Socials:
[![Facebook](https://img.shields.io/badge/Facebook-%231877F2.svg?logo=Facebook&logoColor=white)](https://facebook.com/www.facebook.com/rizaldy.condino/) [![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://linkedin.com/in/www.linkedin.com/in/rizaldy-condino-b24b3a20b/) 

# 💻 Tech Stack:

## 🚀 Frontend

![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white)
![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Zustand](https://img.shields.io/badge/Zustand-%23000000.svg?style=for-the-badge&logo=react&logoColor=white)
![Vue.js](https://img.shields.io/badge/vue.js-%2335495e.svg?style=for-the-badge&logo=vuedotjs&logoColor=%234FC08D)

## ⚙️ Backend / Services
![Stripe](https://img.shields.io/badge/Stripe-626CD9?style=for-the-badge&logo=stripe&logoColor=white)
![Clerk](https://img.shields.io/badge/Clerk-3A3A3A?style=for-the-badge&logo=clerk&logoColor=white)
![Laravel](https://img.shields.io/badge/laravel-%23FF2D20.svg?style=for-the-badge&logo=laravel&logoColor=white)

## 🗄️ Database / CMS
![Prisma](https://img.shields.io/badge/Prisma-3982CE?style=for-the-badge&logo=prisma&logoColor=white)
![Neon](https://img.shields.io/badge/Neon-00E699?style=for-the-badge&logo=postgresql&logoColor=white)
![Sanity](https://img.shields.io/badge/Sanity-F03E2F?style=for-the-badge&logo=sanity&logoColor=white)
![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white)

## 🧠 State & Data Flow
- Zustand (Cart, UI state, favorites)
- Server Actions / API Routes (Next.js)
- Stripe Webhooks (Order & Inventory sync)

## 🛠️ Tools
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
![Vercel](https://img.shields.io/badge/vercel-%23000000.svg?style=for-the-badge&logo=vercel&logoColor=white)

[![](https://visitcount.itsvg.in/api?id=RizaldyCondino&icon=0&color=0)](https://visitcount.itsvg.in)

# 🚀 Recent Projects:

<img width="800" height="450" alt="Image" src="https://github.com/user-attachments/assets/003bdcb2-0485-4c32-898c-72feff642b9a" />

# 🛒 E-Commerce OzCrtz  

<img width="800" height="450" alt="Image" src="https://github.com/user-attachments/assets/f5bde018-8c19-48b4-b361-c9cc9dab569b" />

<h1>Architecture Flow</h1>
 
Users can browse products, categories, and product details without logging in, providing a seamless shopping experience for visitors. However, actions that require user-specific data—such as adding products to favorites, accessing saved favorites, managing account information, and proceeding to checkout—require authentication. When a user attempts to add a product to their favorites or start the checkout process, the application verifies that they are signed in. If they are not authenticated, they are redirected to the login flow.

Before checkout, the application also validates that the user has provided a complete shipping address. This ensures that orders cannot be submitted without the necessary delivery information.

Once validation passes, the application sends the authenticated user's cart data, selected product variants (including size and color selections), and shipping information to a secure server endpoint. The server creates a Stripe Checkout Session and returns the session URL to the client. The user is then redirected to Stripe's hosted checkout page, where payment is processed securely.

After a successful payment, Stripe sends a `checkout.session.completed` webhook event to the backend. The webhook verifies the event's authenticity, creates the order record, and stores the complete order details. It then updates inventory quantities in Sanity, reducing stock based on the exact product variants purchased, including color and size combinations. Any applicable discounts are reflected in the final order calculation.

This webhook-driven architecture ensures that inventory updates only occur after Stripe confirms a successful payment, preventing stock inconsistencies caused by abandoned or failed checkout attempts. Additionally, authenticated users can maintain personalized data such as favorites, shipping addresses, and order history across sessions, creating a more complete e-commerce experience.

 🚀 Frontend

![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white)
![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Zustand](https://img.shields.io/badge/Zustand-%23000000.svg?style=for-the-badge&logo=react&logoColor=white)

 ⚙️ Backend / Services
![Stripe](https://img.shields.io/badge/Stripe-626CD9?style=for-the-badge&logo=stripe&logoColor=white)
![Clerk](https://img.shields.io/badge/Clerk-3A3A3A?style=for-the-badge&logo=clerk&logoColor=white)

 🗄️ Database / CMS
![Prisma](https://img.shields.io/badge/Prisma-3982CE?style=for-the-badge&logo=prisma&logoColor=white)
![Neon](https://img.shields.io/badge/Neon-00E699?style=for-the-badge&logo=postgresql&logoColor=white)
![Sanity](https://img.shields.io/badge/Sanity-F03E2F?style=for-the-badge&logo=sanity&logoColor=white)

## 🧠 State & Data Flow
- Zustand (Cart, UI state, favorites)
- Server Actions / API Routes (Next.js)
- Stripe Webhooks (Order & Inventory sync)

## 🛠️ Tools
![Vercel](https://img.shields.io/badge/vercel-%23000000.svg?style=for-the-badge&logo=vercel&logoColor=white)



# 🛒 E-Commerce ShopCrtz  

<img width="800" height="450" alt="Image" src="https://github.com/user-attachments/assets/a9e6f48c-611f-40b6-9c84-c6f86784c48f" />

🔗 **[Demo: ShopCrtz](https://shopcrtz.vercel.app/)**

A full-stack ecommerce web application built with modern technologies including Next.js, React, and TypeScript. The project demonstrates a complete online shopping system with product browsing, category filtering, authentication, shopping cart functionality, and secure payments using Stripe. It integrates a backend database for managing products and orders, along with state management for seamless user experience. The application follows production-ready practices and is deployed on Vercel.


#🛠️ Tech Stack

🚀 Frontend
Next.js – Full-stack React framework for SSR and routing
React – UI component-based library
TypeScript – Type-safe JavaScript development
Tailwind CSS – Utility-first styling for modern UI

⚙️ Backend
Next.js API Routes – Server-side logic and endpoints
Node.js – JavaScript runtime environment

🗄️ Database & CMS
Prisma – Type-safe ORM for database management
Neon / PostgreSQL – Serverless database solution
Sanity.io – Headless CMS for product/content management

🔐 Authentication
Clerk – User authentication and session management

💳 Payments
Stripe – Secure payment processing and checkout system

🧠 State Management
Zustand – Lightweight global state management (cart, UI state)

☁️ Deployment
Vercel – Hosting and deployment for Next.js applications
GitHub – Version control and CI/CD integration



🛒 **E-Commerce Web App | Laravel + Vue.js + Inertia + Stripe**

🔗 **[Demo: Ecommerce](https://youtu.be/7Sop-O-YO8Q)**

  ![Image](https://github.com/user-attachments/assets/d72c3c48-c335-48c6-b5bd-c4540f6a350b)
 💻 **GitHub Repository:** [Ecommerce Project](https://github.com/RizaldyCondino/Ecommerce)

Welcome to my full-stack **E-Commerce Web Application** built using modern web technologies! This project demonstrates a complete online shopping experience — from browsing products to secure checkout.

🚀 **Tech Stack Used:**

* ⚙️ Laravel Breeze (Authentication)
* 🎨 Vue.js (Frontend)
* 🔗 Inertia.js (SPA experience without API complexity)
* 💳 Stripe (Secure online payments)
* 🎯 Flowbite (UI components & styling)
* 🔔 SweetAlert2 (Beautiful alerts & notifications)

✨ **Key Features:**

* 🛍️ Product listing with categories & brand filtering
* 🔎 Dynamic filtering with debounce search
* 🛒 Add to cart & cart management system
* 💰 Secure checkout with Stripe payment integration
* 🔐 User authentication (Login/Register)
* 📦 Order processing workflow
* ⚡ Smooth SPA experience using Inertia.js

📌 **What I Learned:**

* Building a full-stack application with Laravel & Vue
* Handling state and routing with Inertia.js
* Integrating third-party payment systems (Stripe)
* Creating responsive UI with Flowbite
* Improving UX with SweetAlert notifications

---

📦 Employee Management System
📌 Status: 🟡 In Progress (Not yet completed)

This project is currently under development and will continue to be improved with additional features and refinements.
A full-featured Employee Management System designed to handle core HR operations such as employee records, departments, leave requests, payroll, attendance tracking, and company announcements.
- Built with **Laravel + MySQL**
- 📌 Focus: Backend logic & database relationships
🚀 Project Preview
 <img width="800" height="450" alt="Image" src="https://github.com/user-attachments/assets/7f297e1b-a34a-44bc-b8c2-9bd172142f39" />

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

If you want, I can also help you upgrade this into a fully professional GitHub README (with badges, tech stack icons, features section, and deployment guide).
