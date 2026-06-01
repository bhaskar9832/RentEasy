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
│   └── system-design.md
│
├── frontend/
│   ├── package.json
│   ├── vite.config.js
│   ├── index.html
│   ├── .env.example
│   │
│   └── src/
│       ├── main.jsx
│       ├── App.jsx
│       │
│       ├── assets/
│       │   ├── images/
│       │   └── icons/
│       │
│       ├── components/
│       │   ├── common/
│       │   │   ├── Navbar.jsx
│       │   │   ├── Footer.jsx
│       │   │   ├── Button.jsx
│       │   │   ├── Input.jsx
│       │   │   ├── Modal.jsx
│       │   │   └── Loader.jsx
│       │   │
│       │   ├── listing/
│       │   │   ├── ListingCard.jsx
│       │   │   ├── ListingFilter.jsx
│       │   │   ├── ListingGallery.jsx
│       │   │   └── AmenityBadge.jsx
│       │   │
│       │   ├── booking/
│       │   │   ├── BookingForm.jsx
│       │   │   └── BookingSummary.jsx
│       │   │
│       │   └── dashboard/
│       │       ├── Sidebar.jsx
│       │       └── StatsCard.jsx
│       │
│       ├── pages/
│       │   ├── Home.jsx
│       │   ├── Login.jsx
│       │   ├── Register.jsx
│       │   ├── SearchResults.jsx
│       │   ├── ListingDetails.jsx
│       │   ├── StudentDashboard.jsx
│       │   ├── OwnerDashboard.jsx
│       │   ├── AddListing.jsx
│       │   ├── ManageListings.jsx
│       │   ├── MyBookings.jsx
│       │   └── AdminDashboard.jsx
│       │
│       ├── routes/
│       │   ├── AppRoutes.jsx
│       │   └── ProtectedRoute.jsx
│       │
│       ├── services/
│       │   ├── api.js
│       │   ├── authService.js
│       │   ├── listingService.js
│       │   ├── bookingService.js
│       │   ├── paymentService.js
│       │   └── uploadService.js
│       │
│       ├── context/
│       │   ├── AuthContext.jsx
│       │   └── AppContext.jsx
│       │
│       ├── hooks/
│       │   ├── useAuth.js
│       │   ├── useListings.js
│       │   └── useBookings.js
│       │
│       ├── utils/
│       │   ├── constants.js
│       │   ├── validators.js
│       │   ├── formatDate.js
│       │   ├── formatCurrency.js
│       │   └── errorHandler.js
│       │
│       └── styles/
│           ├── index.css
│           └── responsive.css
│
├── backend/
│   ├── package.json
│   ├── server.js
│   ├── app.js
│   ├── .env.example
│   │
│   └── src/
│       ├── config/
│       │   ├── db.js
│       │   ├── redis.js
│       │   ├── cloudinary.js
│       │   ├── razorpay.js
│       │   └── jwt.js
│       │
│       ├── modules/
│       │   ├── auth/
│       │   │   ├── auth.controller.js
│       │   │   ├── auth.service.js
│       │   │   ├── auth.routes.js
│       │   │   ├── auth.validator.js
│       │   │   └── auth.model.js
│       │   │
│       │   ├── users/
│       │   │   ├── user.controller.js
│       │   │   ├── user.service.js
│       │   │   ├── user.routes.js
│       │   │   └── user.model.js
│       │   │
│       │   ├── listings/
│       │   │   ├── listing.controller.js
│       │   │   ├── listing.service.js
│       │   │   ├── listing.routes.js
│       │   │   ├── listing.validator.js
│       │   │   └── listing.model.js
│       │   │
│       │   ├── rooms/
│       │   │   ├── room.controller.js
│       │   │   ├── room.service.js
│       │   │   ├── room.routes.js
│       │   │   └── room.model.js
│       │   │
│       │   ├── bookings/
│       │   │   ├── booking.controller.js
│       │   │   ├── booking.service.js
│       │   │   ├── booking.routes.js
│       │   │   ├── booking.validator.js
│       │   │   └── booking.model.js
│       │   │
│       │   ├── payments/
│       │   │   ├── payment.controller.js
│       │   │   ├── payment.service.js
│       │   │   ├── payment.routes.js
│       │   │   └── payment.model.js
│       │   │
│       │   ├── reviews/
│       │   │   ├── review.controller.js
│       │   │   ├── review.service.js
│       │   │   ├── review.routes.js
│       │   │   └── review.model.js
│       │   │
│       │   └── uploads/
│       │       ├── upload.controller.js
│       │       ├── upload.service.js
│       │       └── upload.routes.js
│       │
│       ├── middlewares/
│       │   ├── authMiddleware.js
│       │   ├── roleMiddleware.js
│       │   ├── errorMiddleware.js
│       │   ├── validateMiddleware.js
│       │   ├── uploadMiddleware.js
│       │   └── rateLimitMiddleware.js
│       │
│       ├── utils/
│       │   ├── ApiError.js
│       │   ├── ApiResponse.js
│       │   ├── asyncHandler.js
│       │   ├── generateToken.js
│       │   ├── hashPassword.js
│       │   └── logger.js
│       │
│       ├── database/
│       │   ├── migrations/
│       │   ├── seeds/
│       │   └── schema.sql
│       │
│       └── tests/
│           ├── unit/
│           ├── integration/
│           └── e2e/
│
├── nginx/
│   └── nginx.conf
│
├── deployment/
│   ├── Dockerfile.frontend
│   ├── Dockerfile.backend
│   ├── docker-compose.prod.yml
│   ├── render.yaml
│   ├── railway.json
│   └── vercel.json
│
└── scripts/
    ├── setup.sh
    ├── seed-db.sh
    └── reset-db.sh
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
