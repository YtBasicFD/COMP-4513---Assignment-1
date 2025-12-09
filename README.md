# COMP-4513-Assignment-2
# 📌 Overview

This project is a single-page React application built for COMP 4513 (Winter 2025) Assignment 2.
It functions as a small online storefront where users can:

- Browse products

- View product details

- Add/remove items from a shopping cart

- Authenticate using mock login

- Access an admin-only dashboard

The app is built according to Option 2 specifications and follows best practices in React, context management, and modular UI design.

## ✨ Features
### 🛍️ Product Catalog

- Product list view

- Individual product detail pages

- Displays title, price, stock, description, and images

- Data loaded via a service file from the provided API

### 🛒 Shopping Cart (Global State)

- Managed using CartContext

- Add/remove items from anywhere

Cart page shows:

- item list

- product images

- remove buttons

- running total

- Cart persists in localStorage

### 🔐 Authentication (Modal Login)

- Implemented using AuthContext

- LoginView shows inside a Modal pop-out

After successful login:

- modal closes automatically

- header updates to show Logged In + username

- Includes admin and guest accounts

### 🖥️ Admin Dashboard (Protected Route)

Only accessible to admin users

Displays:

- total products

- average price

- total inventory value

- top 5 highest-priced products

### 💬 About Dialog

- Shown as a modal pop-out

- Uses shared Modal component

### 🎨 Tailwind UI

- Utility classes used throughout

- Clean, consistent design

- Mobile-responsive layout

### 🔑 Login Credentials
| User  | Username | Password    | Role                 |
| ----- | -------- | ----------- | -------------------- |
| Admin | `admin`  | `adminpass` | Can access dashboard |
| Guest | `guest`  | `guestpass` | Regular user         |