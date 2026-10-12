# 🏢 Resource Reservation Management System

A practical, full-stack web application designed to centralize and simplify the management of shared organizational facilities, equipment, and resources. Built as a technical assessment for the Software Engineering Internship at PrimeWave Lab (Pvt) Ltd.

---

## ✨ Features

* **Centralized Resource Management:** Browse, view, and manage shared organization resources (e.g., meeting rooms, equipment, hardware) categorized by type, location, and capacity.
* **Conflict-Free Reservation System:** Schedule resource bookings with strict validation logic to prevent **double-booking** over overlapping time slots.
* **User & Role Management:** Seamless support for tracking users and organizing bookings by personnel.
* **Real-Time Validation & Feedback:** Instant UI feedback powered by Zod validation and structured API error handling.

---

## 🛠️ Tech Stack

* **Framework:** [Next.js 16 (App Router)](https://nextjs.org/) with TypeScript
* **Styling:** [Tailwind CSS](https://tailwindcss.com/)
* **Database & ORM:** [PostgreSQL](https://www.postgresql.org/) with [Prisma ORM](https://www.prisma.io/)
* **Validation:** [Zod](https://zod.dev/)
* **Version Control:** Git & GitHub

---

## 📂 Project Structure

```text
src/
├── app/
│   ├── api/                 # Backend API Routes
│   │   ├── resources/       # GET, POST Resource endpoints
│   │   ├── reservations/    # GET, POST Reservation & conflict-checking endpoints
│   │   └── users/           # GET Users endpoint
│   ├── layout.tsx           # Root layout with global styles
│   └── page.tsx             # Main Dashboard UI
├── components/              # Reusable UI components (Navbar, etc.)
└── lib/                     # Database client configuration (Prisma singleton)
