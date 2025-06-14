# 🎯 OAuth Frontend – GitHub & Google Login Interface

![Vite](https://img.shields.io/badge/Vite-Frontend-blueviolet?logo=vite)
![React](https://img.shields.io/badge/React-18+-brightgreen?logo=react)
![Vercel](https://img.shields.io/badge/Hosted_on-Vercel-black?logo=vercel)

A clean and minimal frontend built with **React + Vite** to demonstrate OAuth 2.0 login via **GitHub** and **Google**, powered by a secure custom backend.

---

## 🚀 Live Demo

| Platform    | URL                                                                        |
| ----------- | -------------------------------------------------------------------------- |
| 🌐 Frontend | [oauth-frontend-eac27.vercel.app](https://oauth-frontend-eac27.vercel.app) |
| 🔐 Backend  | [oauth-server-eac27.vercel.app](https://oauth-server-eac27.vercel.app)     |

---

## 📋 Table of Contents

- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Run Locally](#-run-locally)
- [Environment Variables](#-environment-variables)
- [How It Works](#-how-it-works)
- [Folder Structure](#-folder-structure)
- [Backend Repository](#-backend-repository)
- [License](#-license)

---

## ✨ Features

- 🔘 Login with GitHub and Google
- ⚙️ Communicates with custom backend to set secure cookies
- 🔐 Fetches user profile after login
- 🚀 Deployed via Vercel

---

## 🛠 Tech Stack

- **React 18+** (via Vite)
- **Axios** for API communication
- **Vercel** for deployment
- **React Router** for route management

---

## 💻 Run Locally

Clone the frontend project:

```bash
git clone https://github.com/ajmal92786/oauth-frontend.git
cd oauth-frontend
npm install
```

Start the dev server:

```bash
npm run dev
```

🧪 Backend should run at: `http://localhost:4000`
Frontend should run at: `http://localhost:3000`

---

## 🧾 Environment Variables

Create a `.env` file in the root of the frontend:

```env
VITE_SERVER_BASE_URL=http://localhost:4000
VITE_GITHUB_API_BASE_URL=https://api.github.com
```

📂 Add a `.env.example` file for collaborators.

---

## 🔄 How It Works

1. User clicks **Login with GitHub** or **Login with Google**.
2. Redirects to the backend → which redirects to the provider.
3. After login, backend sets `access_token` in HTTP-only cookie.
4. Frontend fetches the profile using `/user/profile/github` or `/user/profile/google`.
5. Displays profile information on screen.

---

## 📁 Folder Structure

```
oauth-frontend/
├── public/
├── src/
│   ├── assets/
│   ├── components/
│   │    ├── Home/
│   │    ├── OwnerProfile/
│   │    └── index.js
│   ├── lib/
│   │    ├── axios.lib.js
│   │    └── index.js
│   ├── App.jsx
│   ├── main.jsx
│   └── index.css
├── .env.example
├── .gitignore
├── eslint.config.js
├── index.html
├── package-lock.json
├── package.json
├── postcss.config.js
├── tailwind.config.js
├── vite.config.js
├── vercel.json
└── README.md
```

---

## 🧠 Backend Repository

This app relies on the backend OAuth server:

🔗 [Backend Repo](https://github.com/ajmal92786/oauth-server)
🔧 [Backend Live URL](https://oauth-server-eac27.vercel.app)

---

## 📄 License

This project is for educational/demo purposes. Feel free to fork, clone, and build on top of it.

---
