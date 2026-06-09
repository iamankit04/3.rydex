<div align="center">

# 🚗 Rydex

### Multi-Partner Vehicle Booking Platform

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Visit-brightgreen?style=for-the-badge&logo=vercel)](https://3-rydex-nu.vercel.app)
[![GitHub](https://img.shields.io/badge/Source%20Code-GitHub-181717?style=for-the-badge&logo=github)](https://github.com/iamankit04/3.rydex)
[![Next.js](https://img.shields.io/badge/Next.js-black?style=for-the-badge&logo=next.js)](https://nextjs.org)
[![TypeScript](https://img.shields.io/badge/TypeScript-blue?style=for-the-badge&logo=typescript)](https://www.typescriptlang.org)

A full-stack, multi-role vehicle booking platform with real-time tracking, automated revenue splitting, video KYC, and AI-powered in-ride chat.

</div>

---

## 📸 Overview

Rydex is a production-grade vehicle booking platform that connects **Users**, **Partners (Drivers)**, and **Admins** through dedicated role-based dashboards. It handles the full booking lifecycle — from ride request and payment to real-time tracking and OTP-verified drop-off — with a clean, scalable architecture.

---

## ✨ Features

### 👤 User
- Book rides with real-time driver tracking
- Secure Google OAuth & email/OTP login
- In-ride AI-powered chat with driver
- OTP-verified pickup and drop confirmation

### 🚘 Partner (Driver)
- Dedicated onboarding with document & image upload via Cloudinary
- Video KYC verification with admin
- Manage ride requests and earnings dashboard
- Automated 90/10 revenue split via Razorpay

### 🛡️ Admin
- Approve/reject partner onboarding and KYC
- Full platform oversight and role management
- Revenue and booking analytics dashboard

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| **Frontend** | Next.js, TypeScript, Tailwind CSS, GSAP |
| **Backend** | Next.js API Routes, Node.js |
| **Database** | MongoDB, Mongoose |
| **Auth** | NextAuth.js (Google OAuth + Email/OTP) |
| **Payments** | Razorpay (automated revenue split) |
| **State Management** | Redux Toolkit (async thunks) |
| **Media & Docs** | Cloudinary |
| **Video KYC** | Jigo Cloud |
| **AI Chat** | AI-powered in-ride support |

---

## 🏗️ Architecture Highlights

- **Role-Based Access Control** — Middleware-enforced routing for User, Partner, and Admin roles via Next.js middleware
- **Automated Revenue Split** — Razorpay integration auto-distributes 90% to partner, 10% to admin on every booking
- **Real-Time Tracking** — Live ride status updates with pickup/drop OTP verification
- **Secure KYC Flow** — Partners submit business documents via Cloudinary; video KYC handled through Jigo Cloud
- **Global State** — Redux Toolkit slices manage vehicle, user, and onboarding data with custom async hooks

---

## 🚀 Getting Started

### Prerequisites
- Node.js 18+
- MongoDB instance (local or Atlas)
- Razorpay, Cloudinary, and NextAuth credentials

### Installation

```bash
# Clone the repository
git clone https://github.com/iamankit04/3.rydex.git
cd 3.rydex

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env.local
# Fill in your credentials in .env.local

# Run the development server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to view the app.

### Environment Variables

```env
NEXTAUTH_SECRET=
NEXTAUTH_URL=

GOOGLE_CLIENT_ID=
GOOGLE_CLIENT_SECRET=

MONGODB_URI=

RAZORPAY_KEY_ID=
RAZORPAY_KEY_SECRET=

CLOUDINARY_CLOUD_NAME=
CLOUDINARY_API_KEY=
CLOUDINARY_API_SECRET=

JIGO_API_KEY=
```

---

## 📁 Project Structure

```
rydex/
├── app/                  # Next.js App Router pages & API routes
│   ├── (user)/           # User-facing pages
│   ├── (partner)/        # Partner dashboard
│   ├── (admin)/          # Admin dashboard
│   └── api/              # API route handlers
├── components/           # Reusable UI components
├── lib/                  # DB connection, utilities, helpers
├── store/                # Redux Toolkit slices & store config
├── middleware.ts          # Role-based route protection
└── public/               # Static assets
```

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to open an issue or submit a pull request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📬 Contact

**Ankit Kumar Gupta**
- 📧 [ankitkumargup143@gmail.com](mailto:ankitkumargup143@gmail.com)
- 💼 [linkedin.com/in/iamankit04](https://linkedin.com/in/iamankit04)
- 🐙 [github.com/iamankit04](https://github.com/iamankit04)

---

<div align="center">

*Built with ❤️ by Ankit Kumar Gupta*

</div>
