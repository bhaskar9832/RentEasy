# 🏠 RentEasy

### Student Accommodation Finder Platform

<div align="center">

<img src="./Renteasy.png" alt="RentEasy Logo" width="320" />

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
renteasy/
│
├── README.md
├── .gitignore
├── .env.example
├── docker-compose.yml
│
├── docs/
│   ├── synopsis.pdf
│   ├── api-documentation.md
│   ├── database-design.md
│   ├── system-design.md
│   └── architecture-diagram.png
│
├── apps/
│   │
│   ├── web/
│   │   ├── public/
│   │   ├── src/
│   │   │   ├── assets/
│   │   │   ├── api/
│   │   │   │   ├── auth.js
│   │   │   │   ├── users.js
│   │   │   │   ├── listings.js
│   │   │   │   ├── bookings.js
│   │   │   │   └── search.js
│   │   │   │
│   │   │   ├── components/
│   │   │   │   ├── common/
│   │   │   │   ├── listing/
│   │   │   │   ├── booking/
│   │   │   │   └── dashboard/
│   │   │   │
│   │   │   ├── context/
│   │   │   ├── hooks/
│   │   │   ├── pages/
│   │   │   │   ├── Home.jsx
│   │   │   │   ├── Login.jsx
│   │   │   │   ├── Register.jsx
│   │   │   │   ├── Search.jsx
│   │   │   │   ├── ListingPage.jsx
│   │   │   │   ├── BookingPage.jsx
│   │   │   │   ├── Profile.jsx
│   │   │   │   ├── OwnerPortal.jsx
│   │   │   │   └── AdminDashboard.jsx
│   │   │   │
│   │   │   ├── routes/
│   │   │   ├── styles/
│   │   │   ├── utils/
│   │   │   ├── App.jsx
│   │   │   └── main.jsx
│   │   │
│   │   ├── package.json
│   │   ├── vite.config.js
│   │   └── .env
│   │
│   └── mobile/
│
├── services/
│   │
│   ├── api-gateway/
│   │   ├── src/
│   │   │   ├── routes/
│   │   │   ├── middleware/
│   │   │   └── server.js
│   │   ├── package.json
│   │   └── .env
│   │
│   ├── auth-service/
│   │   ├── src/
│   │   │   ├── controllers/
│   │   │   ├── routes/
│   │   │   ├── services/
│   │   │   ├── middleware/
│   │   │   └── server.js
│   │   ├── package.json
│   │   └── .env
│   │
│   ├── user-service/
│   │   ├── src/
│   │   │   ├── controllers/
│   │   │   ├── routes/
│   │   │   ├── services/
│   │   │   ├── config/
│   │   │   └── server.js
│   │   ├── package.json
│   │   └── .env
│   │
│   ├── catalog-service/
│   │   ├── src/
│   │   │   ├── controllers/
│   │   │   ├── routes/
│   │   │   ├── services/
│   │   │   └── server.js
│   │   ├── package.json
│   │   └── .env
│   │
│   ├── booking-service/
│   │   ├── src/
│   │   │   ├── controllers/
│   │   │   ├── routes/
│   │   │   ├── services/
│   │   │   └── server.js
│   │   ├── package.json
│   │   └── .env
│   │
│   ├── search-service/
│   │   ├── src/
│   │   │   ├── controllers/
│   │   │   ├── routes/
│   │   │   ├── services/
│   │   │   └── server.js
│   │   ├── package.json
│   │   └── .env
│   │
│   ├── notification-service/
│   │   ├── src/
│   │   │   ├── services/
│   │   │   ├── consumers/
│   │   │   └── server.js
│   │   ├── package.json
│   │   └── .env
│   │
│   └── payment-service/
│       ├── src/
│       │   ├── controllers/
│       │   ├── routes/
│       │   ├── services/
│       │   └── server.js
│       ├── package.json
│       └── .env
│
├── shared/
│   ├── constants/
│   ├── middleware/
│   ├── utils/
│   └── validation/
│
├── database/
│   ├── migrations/
│   ├── schemas/
│   └── seeds/
│
├── infra/
│   ├── docker/
│   ├── k8s/
│   ├── terraform/
│   └── monitoring/
│
└── .github/
└── workflows/
├── ci.yml
├── cd.yml
└── deploy.yml

```
# 📂 Another Folder Structure

```bash


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
