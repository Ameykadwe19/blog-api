# 📝 Blog Website

A simple blog website where users can create, update, and delete blog posts. Built using **Node.js**, **Express.js**, **EJS**, and other technologies with local in-memory data handling (no database). 

---

## 🌟 Features

- Create and delete blog posts
- Edit blog content, author name, and title
- View all blog entries dynamically
- Rendered using **EJS** templates
- No database — data is stored in memory (resets on restart)
- Communicates via **API** calls between frontend and backend

---

## 🔧 Tech Stack

- **Node.js** – JavaScript runtime for the server-side.
- **Express.js** – Web framework for handling HTTP requests and routing.
- **EJS** – Embedded JavaScript templating for dynamic content rendering.
- **Axios** – Promise-based HTTP client for API requests.
- **body-parser** – Middleware for parsing incoming request bodies in JSON format.
- **Nodemon** – Utility for automatically restarting the server during development.

---

## 🚀 Getting Started

### 1. Clone the Repository

First, clone the repository to your local machine:

```bash
git clone https://github.com/Ameykadwe19/blog-api.git
cd blog-api
```

### 2. 📦 Install Dependencies

To install all the required dependencies, run this one-liner:

```bash
npm install express ejs axios body-parser nodemon
```

### 3. 🚀 Run the App in Development Mode

For an **easy setup** to run the app with **auto-reloading** (using `nodemon`), just run:

```bash
npx nodemon app.js
```

This will start your **frontend server** on `http://localhost:3000`.

If you have a **second server** (e.g., for handling API requests), you can run it with:

```bash
npx nodemon server.js
```

Make sure the second server (if applicable) runs on a **different port** (e.g., `4000`).

> ⚠️ **Important**: Ensure both servers are running on **different ports** to avoid conflicts.

---

### 🔗 How the Servers Work Together

- **Frontend Server** (`http://localhost:3000`) renders the HTML using **EJS** templates.
- **API Server** (`http://localhost:4000`) handles the logic for managing blog posts (create, update, delete, view), often by making **API calls** (via **Axios**) to retrieve and send data.
- **Axios** is used in the frontend to send requests to the API, and **Express.js** handles the routing and requests on the backend.

---

## 📄 License

This project is licensed under the MIT License.
