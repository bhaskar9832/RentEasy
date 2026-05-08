# 🏠 RentEasy

### Student Accommodation Finder Platform

<div align="center">

![RentEasy Banner](./assets/renteasy-ui.png)

### Find PGs, hostels, and mess facilities near your college.

</div>

---

# 📌 About The Project

RentEasy is a student-focused accommodation finder platform built to simplify the process of searching for PGs, hostels, and mess facilities near colleges and universities.

Most existing real-estate platforms are designed mainly for apartments and family housing, which creates problems for students looking for affordable and flexible accommodation.

RentEasy solves this problem by providing:

* Student-focused accommodation listings
* Real-time room availability
* Transparent pricing and amenities
* Food and mess information
* Online booking system
* Secure authentication
* Owner property management system

This project is currently under active development as a Final Year B.Tech Project.

---

# 🚀 UI Preview

## Landing Page

<img src="./Untitled%20design%20(1).png" alt="RentEasy UI" width="100%" />
---

# ✨ Features

## 👨‍🎓 Student Features

* Search PGs and hostels near colleges
* Filter by:

  * Budget
  * Food included
  * Single/shared room
  * Location
* Real-time room availability
* Ratings and reviews
* Property photos and amenities
* Secure login/signup
* Online booking system
* Responsive UI for mobile and desktop

## 🏢 Owner Features

* Add and manage property listings
* Upload room photos
* Manage room availability
* Update pricing and amenities
* View booking requests
* Manage student interactions

---

# 🛠️ Tech Stack

## Frontend

* React.js
* Tailwind CSS
* Vite
* Flutter (Mobile App)

## Backend

* Node.js
* Express.js
* REST API
* JWT Authentication

## Database

* PostgreSQL

## Caching

* Redis

## Search Engine

* Elasticsearch

## Cloud & Storage

* AWS S3

## Payment Integration

* Razorpay
* PayPal

## Deployment & DevOps

* Docker
* Kubernetes
* GitHub Actions (CI/CD)

## Monitoring

* Prometheus
* Grafana

---

# 🧱 System Architecture

RentEasy follows a scalable microservices-inspired architecture.

### Main Services

* Authentication Service
* Property Listing Service
* Booking Service
* Payment Service
* Notification Service
* Search Service

The system is designed for scalability and future expansion across multiple cities and colleges.

---

# 📂 Proposed Folder Structure

```bash
RentEasy/
│
├── client/                     # React Frontend
│   ├── public/
│   ├── src/
│   │   ├── assets/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── layouts/
│   │   ├── hooks/
│   │   ├── context/
│   │   ├── services/
│   │   ├── utils/
│   │   └── App.jsx
│   └── package.json
│
├── server/                     # Backend API
│   ├── src/
│   │   ├── config/
│   │   ├── controllers/
│   │   ├── middleware/
│   │   ├── models/
│   │   ├── routes/
│   │   ├── services/
│   │   ├── utils/
│   │   └── app.js
│   └── package.json
│
├── mobile-app/                 # Flutter App
│
├── docs/                       # Documentation
│
├── assets/                     # Screenshots & UI images
│   └── renteasy-ui.png
│
├── docker-compose.yml
├── README.md
└── .env
```

---

# ⚙️ Installation & Setup

## Clone Repository

```bash
git clone https://github.com/bhaskar9832/RentEasy.git
cd RentEasy
```

## Install Dependencies

### Frontend

```bash
cd client
npm install
npm run dev
```

### Backend

```bash
cd server
npm install
npm run dev
```

---

# 🎯 Problem Statement

Students often struggle to find suitable accommodation because:

* Existing real-estate platforms are not designed for students
* Listings are outdated or incomplete
* Affordable shared rooms are difficult to find
* Student-friendly amenities are not highlighted properly
* Short-term stays are usually unavailable
* Students often depend on brokers and unreliable information

RentEasy aims to solve these issues with a transparent and student-focused platform.

---

# 📈 Future Plans

* AI-based accommodation recommendations
* Roommate matching system
* Google Maps integration
* Chat system between students and owners
* Mobile app deployment
* Smart analytics dashboard
* College-specific communities

---

# 📖 Documentation

Project documentation, ER diagrams, system design, and reports will be added inside the `/docs` folder.

---

# 📸 Screenshots

## Homepage UI

<img src="./assets/renteasy-ui.png" alt="Homepage UI" width="100%" />

---

# 📚 References

* Node.js Documentation
* React Documentation
* PostgreSQL Documentation
* Redis Documentation
* Elasticsearch Documentation
* Docker Documentation
* Kubernetes Documentation

---

# 📄 License

This project is developed for academic and educational purposes.

---

<div align="center">

### Building a better accommodation experience for students.

⭐ Star the repository if you like the project.

</div>
