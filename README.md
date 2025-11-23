# 🛡️ SafeReport - Anonymous Crime Reporting App

A secure, AI-powered platform for citizens to report incidents anonymously and safely.

![Next.js](https://img.shields.io/badge/Next.js-14-black)
![TypeScript](https://img.shields.io/badge/TypeScript-5.0-blue)
![Prisma](https://img.shields.io/badge/Prisma-5.0-2d3748)
![Gemini AI](https://img.shields.io/badge/AI-Gemini%202.5-8e44ad)

## 📋 Table of Contents

- [🤖 Introduction](#-introduction)
- [⚙️ Tech Stack](#-tech-stack)
- [🔋 Features](#-features)
- [🤸 Quick Start](#-quick-start)
- [🕸️ Environment Setup](#-environment-setup)
- [🚀 Deployment](#-deployment)
- [🤝 Contributing](#-contributing)

---

## 🤖 Introduction

**SafeReport** is a next-generation civic safety application built with **Next.js 14**. It empowers users to report crimes or civic issues without compromising their identity. 

The platform leverages **Google Gemini AI** to automatically analyze uploaded evidence images to categorize severity and extract details, ensuring authorities get accurate information faster.

---

## ⚙️ Tech Stack

- **Framework:** Next.js 14 (App Router)
- **Language:** TypeScript
- **Database:** PostgreSQL (via Neon DB)
- **ORM:** Prisma
- **Authentication:** NextAuth.js
- **Styling:** Tailwind CSS
- **AI Analysis:** Google Gemini API (2.5 Flash/Pro)
- **Maps:** Mapbox GL
- **Forms:** React Hook Form

---

## 🔋 Features

- **🔒 Total Anonymity:** Secure reporting flow without forced user registration.
- **🧠 AI-Powered Analysis:** Uses Gemini AI to scan uploaded images and auto-generate incident descriptions and severity ratings.
- **📍 Location Intelligence:** Interactive maps to pin exact incident locations using Mapbox.
- **📱 Responsive Design:** Fully optimized for mobile and desktop reporting.
- **🛡️ Admin Dashboard:** Secure panel for authorities to review and manage incoming reports.

---

## 🤸 Quick Start

### Prerequisites
Make sure you have the following installed:
- Node.js (v18+)
- npm or yarn
- Git

### Installation

1. **Clone the repository**
   ```bash
   git clone [https://github.com/your-username/SafeReport.git](https://github.com/your-username/SafeReport.git)
   cd SafeReport

2. **Install dependencies**
   ```bash
   npm install
   
3. **Initialize the database**
   ```bash
   npx prisma generate
    npx prisma migrate dev --name init

4. **Start the development server**
   ```bash
   npm run dev

  ## 🕸️ Environment Setup
Create a .env file in the root directory. You must fill in these values for the app to function correctly:  

     ```bash
      # Database Connection (Neon/Postgres)
    DATABASE_URL="postgresql://user:password@host/dbname?sslmode=require"
    
    # NextAuth Configuration
    NEXTAUTH_URL="http://localhost:3000"
    NEXTAUTH_SECRET="your-super-secret-key-here"
    
    # Google Gemini AI (Get from Google AI Studio)
    GEMINI_API_KEY="your-gemini-api-key"
    
    # Mapbox (For location features)
    NEXT_PUBLIC_MAPBOX_ACCESS_TOKEN="your-mapbox-public-token"

Tip: You can generate a random NEXTAUTH_SECRET by running openssl rand -base64 32 in your terminal.

# 🚀 Deployment
1.The application is optimized for deployment on Vercel.

2.Push your code to a GitHub repository.

3.Go to Vercel and "Add New Project".

4.Select your repository.

4.Important: Copy all the variables from your .env file into the Vercel Environment Variables section.

5.Click Deploy!
