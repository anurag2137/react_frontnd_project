
# Admin Dashboard - Role-Based Access Control (RBAC)

This project showcases a custom-built **Admin Dashboard** designed and developed by me. It provides role-based access control (RBAC) for admins, creators, and users, ensuring secure and efficient user and content management. Built with modern React techniques, this dashboard is responsive, user-friendly, and highly scalable.

---

## **Table of Contents**
1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Technologies Used](#technologies-used)
4. [Project Structure](#project-structure)
5. [State Management](#state-management)
6. [Routing & Permissions](#routing--permissions)
7. [How to Run the Project](#how-to-run-the-project)
8. [Conclusion](#conclusion)

---

## **Project Overview**

This Admin Dashboard application provides the following features based on roles:

### **Admin Features**
- View, add, and manage users and creators.
- Assign or toggle roles between "User" and "Creator."
- Add new members or roles to the system.

### **Creator Features**
- Create, edit, and manage posts using a rich text editor.
- View and manage previously published posts.

### **User Features**
- Browse and view posts created by creators.
- Follow and unfollow creators for a personalized feed.

---

## **Features**

### **Admin Features**
- **Role Management:** Assign or toggle user roles between "User" and "Creator."
- **User Management:** Add or remove users and creators.

### **Creator Features**
- **Post Creation:** Write and manage posts using the intuitive **TinyMCE** text editor.
- **Post History:** Access previously created posts for review or editing.

### **User Features**
- **Post Viewing:** Explore posts by creators.
- **Follow Creators:** Follow or unfollow creators to customize content visibility.

### **Shared Features**
- **Protected Routes:** Ensure users access only authorized pages based on their roles.
- **Optimized UI:** Smooth loading with shimmer effects and efficient input handling via debounce.
- **Responsive Design:** Fully mobile-friendly layout with a toggleable sidebar.

---

## **Technologies Used**

- **React:** Core framework for creating dynamic and reusable components.
- **React Context API:** For global state management (e.g., roles, posts, and user data).
- **React Router:** Enables navigation and route protection.
- **Reducer:** Centralized state update management.
- **Tailwind CSS:** Simplifies styling for a modern, responsive design.
- **TinyMCE:** Provides a rich text editor for creating and managing posts.
- **Shimmer Effect:** Adds a skeleton loading UI during data fetches.
- **Debounce:** Optimizes input event handling.

---

## **Project Structure**

```
src/
├── components/
│   ├── forms/          # Login and add-user forms
│   ├── CreatorNav/     # Navbar for creators
│   ├── Shimmer/        # Shimmer loading effect component
│   ├── UserNav/        # Navbar for users
├── context/
│   ├── AuthContext/    # Authentication logic
│   ├── BlogContext/    # Blog-related data and actions
├── pages/
│   ├── Dashboard/      # Admin Dashboard
│   ├── Following/      # Follow/unfollow creators (for users)
│   ├── PastBlogs/      # Creator’s blog history
│   ├── UnAuthorized/   # Unauthorized access page
│   ├── UserDashboard/  # User dashboard showing creator posts
│   ├── Write/          # Creator’s post-writing page
├── utils/
│   ├── reducer.js      # Functions for managing state
├── App.jsx             # Contains application routes
├── protectedRoute.jsx  # Protects routes based on roles
```

---

## **State Management**

### **React Context API**
- Manages global state (e.g., user roles, posts, login status).
- Eliminates prop drilling across components.

### **Reducer**
- Centralizes state updates like:
  - Adding or deleting users.
  - Managing roles and posts.

---

## **Routing & Permissions**

### **Protected Routes**
- Ensures role-based access to authorized pages only.
- Redirects unauthorized access to an "Unauthorized" page.

### **Role-Based Permissions**
- **Admin:** Manage users, roles, and access permissions.
- **Creators:** Create and view posts.
- **Users:** View and follow creator posts.

---

## **How to Run the Project**

### **Prerequisites**
Ensure the following are installed:
- **Node.js**
- **npm** or **yarn**

### **Installation Steps**
1. Clone the repository:
   ```bash
   git clone https://github.com/bhardwajankit354/RVAC-VRV.git
   cd admin-dashboard-rbac
   ```

2. Install dependencies:
   ```bash
   npm install
   # or
   yarn install
   ```

3. Start the development server:
   ```bash
   npm start
   # or
   yarn start
   ```

4. Open the application:
   ```
   http://localhost:3000
   ```

---
## Login Details:
1.**[Role: admin]**
    --Email: admin@example.com 
    --Password: admin123 
2.**[Role: user]**
    --Email: user@example.com 
    --Password: user123
3.**[Role: vendor]**
    --Email: creator@example.com 
    --Password: creator123
    ---

## **Conclusion**

This project highlights my ability to implement secure and scalable **Role-Based Access Control (RBAC)** systems. By leveraging React and modern front-end practices, this dashboard provides efficient user and role management features with a responsive and intuitive UI.
