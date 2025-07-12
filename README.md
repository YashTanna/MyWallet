<h1 align="center">🌟 My Wallet - Expense tracking app 🌟</h1>

<p align="center">
  <img alt="Static Badge" src="https://img.shields.io/badge/Spring%20Boot-darkgreen?style=for-the-badge">
  <img alt="Static Badge" src="https://img.shields.io/badge/React.js-blue?style=for-the-badge">
  <img alt="Static Badge" src="https://img.shields.io/badge/mysql-red?style=for-the-badge">
  <img alt="Static Badge" src="https://img.shields.io/badge/css-purple?style=for-the-badge">
  <img alt="Static Badge" src="https://img.shields.io/badge/jwt-orange?style=for-the-badge">
</p>

## Table of contents

1. [Descripiton](#description)
2. [How to run?](#how-to-run)
3. [Screenshots](#screenshots)

## Description

MyWallet is a full-stack web application built using Spring Boot, React.js, and MySQL that helps users manage and track daily expenses. It supports user authentication, role-based dashboards, budget planning, recurring transactions, and real-time analytics.

Features include:
- User/Admin login and role-based access
- Dashboard with transaction and budget summaries
- Secure authentication (sign-up, sign-in, password reset, email verification)
- Category-based expense/income tracking
- Search, filter, pagination, and statistics


## How to run?

### Step 1: Fork and Clone the Repository

1. Fork the repository to your GitHub account.

2. Clone the forked repository to your local machine.

```sh
git clone https://github.com/YashTanna/MyWallet.git
```

### Step 2: Setting up e-mail and database configurations

- Configure the following credentials in the [backend/src/main/resources/application.properties] file.

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/YOUR_DATABASE_NAME
spring.datasource.username=YOUR_USERNAME
spring.datasource.password=YOUR_PASSWORD

spring.mail.username=YOUR_USERNAME
spring.mail.password=YOUR_PASSWORD
```

### Step 3: Run the backend.

- Run the backend application. It will automatically create the required tables. 
- Add some custom data manually in the [categories](https://github.com/DharshiBalasubramaniyam/Fullstack-Expense-Tracker/blob/7ecea71aaeca4e26a4aafd02fd602abe4d9da67d/backend/src/main/java/com/fullStack/expenseTracker/models/Category.java#L13) table for both [type](https://github.com/DharshiBalasubramaniyam/Fullstack-Expense-Tracker/blob/7ecea71aaeca4e26a4aafd02fd602abe4d9da67d/backend/src/main/java/com/fullStack/expenseTracker/models/TransactionType.java#L13) `expense` and `income`.
- To start as admin, Insert a new user manually with role admin in [`users`](https://github.com/DharshiBalasubramaniyam/Fullstack-Expense-Tracker/blob/7ecea71aaeca4e26a4aafd02fd602abe4d9da67d/backend/src/main/java/com/fullStack/expenseTracker/models/User.java#L20) table.

### Step 4: Run the frontend

1. Navigate to [frontend direcory](https://github.com/DharshiBalasubramaniyam/Fullstack-Expense-Tracker/tree/main/frontend).
```
cd ./frontend
```

2. Install dependencies.
```
npm install
```

3. Run the app.
```
npm start
```

Access the application at [`http://localhost:3000/`](http://localhost:3000/).
To get started create a new account using your email.

---

> 💻 Developed by [Yash Tanna](https://github.com/YashTanna)
