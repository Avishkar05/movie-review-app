---

# 🎬 Movie Review Application

A full-stack, cloud-deployed movie review and watchlist application. The backend leverages **Spring Boot** with **Google Sheets** as a cloud database, while the frontend is built with **React** for a seamless user experience. Authentication and authorization are securely managed via **JWT (JSON Web Tokens)**.

---

## 🚀 Live Demo

Click here to visit :  https://cine-reviews.netlify.app/

---

## ✨ Features

* **User Authentication:** Secure signup and login powered by JWT and BCrypt password hashing.
* **Role-Based Access Control (RBAC):**
* **User:** Browse movies, read reviews, submit movie reviews, and manage personal watchlists.
* **Admin:** Full CRUD access to add, update, and delete movies from the catalog.


* **Google Sheets Integration:** Acts as a real-time, zero-cost cloud database via Google Sheets API.
* **Watchlist & Reviews Management:** Synchronous state loading with direct `userId` JWT claims for fast navigation.
* **Responsive UI:** Clean React interface with single-page routing and CORS preflight optimization.

---

## 🛠️ Tech Stack

### **Backend**

* **Language/Framework:** Java 21, Spring Boot 3
* **Security:** Spring Security, JWT (jjwt)
* **Database/Storage:** Google Sheets API
* **Build Tool:** Maven & Docker
* **Hosting:** Render (Web Service / Docker Runtime)

### **Frontend**

* **Framework:** React.js (Hooks, Context API)
* **Routing:** React Router DOM (v6)
* **HTTP Client:** Axios
* **Styling:** CSS3 / Bootstrap
* **Hosting:** Netlify

---

## 📁 Project Structure

```text
movie-review/
├── src/                                # Spring Boot Backend
│   ├── main/
│   │   ├── java/com/
│   │   │   ├── config/                 # SecurityConfig & CORS Bean
│   │   │   ├── controller/             # Review, Watchlist, Movie Controllers
│   │   │   ├── security/               # JwtAuthenticationFilter & UserDetails
│   │   │   └── service/                # Business Logic & Google Sheets Service
│   │   └── resources/
│   │       └── application.properties  # App Settings & Credentials Reference
├── public/                             # Static Frontend Files
│   └── _redirects                      # Netlify SPA Routing Redirects
├── Dockerfile                          # Multi-Stage Docker Container Build Script
├── pom.xml                             # Maven Dependencies
└── package.json                        # React Dependencies

```
