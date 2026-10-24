<div align="center">

  <img src="frontend/public/logo.jpg" alt="MUJMart Logo" width="120" style="border-radius: 24px; box-shadow: 0 8px 30px rgba(0,0,0,0.18);" />

  # 🛒 MUJMart

  ### **The Next-Gen Campus Marketplace & Peer-to-Peer Trading Platform**
  ### *Built exclusively for Manipal University Jaipur (MUJ) Students*

  <p align="center">
    <b>Buy · Sell · Rent · Share · Negotiate — all secured with Escrow-protected UPI transactions.</b>
  </p>

  <p align="center">
    <a href="https://github.com/abhinendrasinghDS/mujmart---in-/stargazers"><img src="https://img.shields.io/github/stars/abhinendrasinghDS/mujmart---in-?style=for-the-badge&logo=starship&color=F59E0B" alt="Stars" /></a>
    <a href="https://github.com/abhinendrasinghDS/mujmart---in-/network/members"><img src="https://img.shields.io/github/forks/abhinendrasinghDS/mujmart---in-?style=for-the-badge&color=3B82F6" alt="Forks" /></a>
    <a href="https://github.com/abhinendrasinghDS/mujmart---in-/issues"><img src="https://img.shields.io/github/issues/abhinendrasinghDS/mujmart---in-?style=for-the-badge&color=10B981" alt="Issues" /></a>
    <img src="https://img.shields.io/badge/License-MIT-purple.svg?style=for-the-badge" alt="License" />
  </p>

  <p align="center">
    <img src="https://img.shields.io/badge/Next.js_16-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js" />
    <img src="https://img.shields.io/badge/React_19-20232A?style=flat-square&logo=react&logoColor=61DAFB" alt="React" />
    <img src="https://img.shields.io/badge/TypeScript_5-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />
    <img src="https://img.shields.io/badge/Tailwind_CSS_4-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white" alt="Tailwind" />
    <img src="https://img.shields.io/badge/Node.js_18+-339933?style=flat-square&logo=nodedotjs&logoColor=white" alt="Node" />
    <img src="https://img.shields.io/badge/Express_4-000000?style=flat-square&logo=express&logoColor=white" alt="Express" />
    <img src="https://img.shields.io/badge/Prisma_5-2D3748?style=flat-square&logo=prisma&logoColor=white" alt="Prisma" />
    <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL" />
    <img src="https://img.shields.io/badge/Socket.io_4-010101?style=flat-square&logo=socketdotio&logoColor=white" alt="Socket.io" />
    <img src="https://img.shields.io/badge/Cloudinary-3448C5?style=flat-square&logo=cloudinary&logoColor=white" alt="Cloudinary" />
    <img src="https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white" alt="JWT" />
    <img src="https://img.shields.io/badge/Jest-C21325?style=flat-square&logo=jest&logoColor=white" alt="Jest" />
  </p>

  <br />

  <p align="center">
    <a href="#-the-problem--our-solution"><b>The Vision</b></a> •
    <a href="#-key-features"><b>Key Features</b></a> •
    <a href="#-system-architecture"><b>Architecture</b></a> •
    <a href="#-transaction--escrow-protocol"><b>Escrow Engine</b></a> •
    <a href="#-tech-stack"><b>Tech Stack</b></a> •
    <a href="#-database-schema--data-models"><b>Database</b></a> •
    <a href="#-api-reference"><b>API Reference</b></a> •
    <a href="#-quickstart-guide"><b>Getting Started</b></a> •
    <a href="#-project-structure"><b>Structure</b></a> •
    <a href="#-roadmap--upcoming-enhancements"><b>Roadmap</b></a>
  </p>

</div>

---

## 💡 The Problem & Our Solution

### ❌ The Campus Problem

At **Manipal University Jaipur (MUJ)**, thousands of hostelers and day-scholars buy, sell, or rent textbooks, electronics, mattresses, kettles, cycles, and lab equipment every semester. However:

- 📱 Deals happen in **cluttered, spam-ridden WhatsApp & Telegram groups** with zero structure.
- 🔒 **No identity verification** leads to scams, ghosting, and unsafe meetups between strangers.
- 💸 Sellers struggle to receive **timely payments**; buyers lack any form of escrow protection.
- 🔍 Chat history gets buried within hours with **no search filters, categories, or listings management**.
- 🤝 No platform for **campus task collaboration** — lab assistance, tutoring, or project work sharing.

### ✅ The MUJMart Solution

**MUJMart** replaces fragmented chat groups with a comprehensive, high-performance, student-exclusive platform:

| Feature | What It Solves |
|---|---|
| 🛡️ **Campus-Only Verified Ecosystem** | Authenticated student profiles with trust scoring (`repScore`) and deal counters |
| 💬 **Live Anonymous Negotiation** | Real-time Socket.io chat that shields personal contact info until a deal is formally locked |
| 💳 **Escrow-Secured Payments** | UPI dynamic QR payments with UTR verification and 5% platform safety margin before seller payout |
| 🔄 **Multi-Mode Commerce** | Sell, Resale, Rent, Free (Giveaways), Task Sharing, and Project Request collaborations |
| ⚖️ **Integrated Dispute Arbitration** | Formal dispute logging and Admin resolution dashboard for complete peace of mind |

---

## ✨ Key Features

### 🛍️ 1. Multi-Tier Marketplace & Discovery

- **Six Comprehensive Listing Modes**:
  | Mode | Description |
  |---|---|
  | `sell` | Direct item sales with instant deal closing |
  | `resale` | Second-hand hostel gear with condition tags (*New, Good, Fair, Damaged*) |
  | `rent` | Short-term lending with return timelines and deposit tracking |
  | `free` | Campus giveaways and donation drives |
  | `share` | Shared study materials, room resources, and rides |
  | `task` | Campus task and project collaboration requests |

- **Rich Media & Attachments**: Upload multi-image galleries and document attachments securely via Cloudinary CDN.
- **Smart Filtering & Search**: Instant full-text search across categories, price bands, condition ratings, and expiry deadlines.
- **Automated Lifecycle Management**: 7-day auto-expiry timers, marking items as `active`, `sold`, `expired`, or `removed`.

---

### 💬 2. Real-Time Negotiation Engine (Socket.io)

- **Direct Listing-Linked Threads**: Every conversation is tied to a specific listing to avoid context loss.
- **Stateful Deal Negotiations**: Real-time deal state machine: `open` ➔ `accepted` ➔ `rejected` ➔ `closed`.
- **Content Masking (`contentGuard`)**: Server-side regex filtering automatically blocks phone numbers and external social handles during anonymous negotiations.
- **Persistent Message Store**: Chat history preserved in PostgreSQL with instant synchronization across all devices.

---

### 💳 3. Escrow Transaction & Margin Engine

- **UPI QR & Reference Generation**: Built-in dynamic UPI payment rendering via `qrcode.react`.
- **UTR & Screenshot Submission**: Buyers upload their UPI transaction reference number (UTR) and payment screenshot for full audit trail.
- **Escrow State Machine**:
  ```
  pending_payment ➔ verifying_payment ➔ escrow ➔ ready_for_payout ➔ completed (or refunded)
  ```
- **Platform Margin Tracking**: Automatic 5% fee calculation recorded per deal for platform sustainability.

---

### 🤝 4. Campus Projects & Task Collaboration

- **Project Request Listings**: Solicit or offer student freelance work, lab assistance, tutoring, and peer study help.
- **Collaborator Workflows**: Accept or reject incoming applications with linked chat threads and real-time notifications.
- **Task Dashboard**: Dedicated `/task` view to manage all ongoing and pending collaborations.

---

### 🔔 5. Notifications & Support Desk

- **In-App Notification Feed**: Real-time alerts for incoming bids, deal approvals, project requests, and dispute updates.
- **Dedicated Help Center**: One-click WhatsApp & email escalation channels, FAQ accordion, and direct ticket submission form.
- **Report Issue Center**: Submit bug reports and marketplace violations with screenshot proof uploads.

---

### 👑 6. Administrator Command Center

- **User Moderation Dashboard**: View all registered students, verify UPI details, inspect reputation scores, and enforce account bans.
- **Dispute Resolution Suite**: Review reporter/defendant chat logs, evaluate evidence, and resolve or dismiss disputes.
- **Financial Oversight**: Audit gross transaction volume, collected platform margins, and pending UPI payouts in real time.
- **Platform Health Metrics**: Live system stats — active listings, total deals, flagged content, and margin revenue.

---

## 🏗 System Architecture

MUJMart uses a clean **Decoupled Monorepo Architecture** separating the modern Next.js client from a scalable Node.js/Express service layer, communicating over REST and WebSockets.

```mermaid
graph TB
    subgraph Client ["🖥️ Client Layer (Next.js 16 + React 19)"]
        UI[Tailwind CSS 4 Responsive UI]
        ChatClient[Socket.io Real-time Client]
        AuthContext[Auth & Session Context]
        QRGen[qrcode.react UPI QR Engine]
    end

    subgraph Gateway ["⚡ API Gateway (Express 4 + TypeScript 5)"]
        Router[REST Route Handlers]
        SocketServer[Socket.io Realtime Engine]
        Security[Helmet + CORS + Rate Limiting]
        AuthGuard[JWT Auth Middleware]
        ContentFilter[contentGuard Filter]
    end

    subgraph Services ["☁️ External & Auxiliary Services"]
        Cloudinary[Cloudinary CDN: Media & Screenshots]
        Firebase[Firebase Client Services]
        Vercel[Vercel Speed & Web Analytics]
    end

    subgraph Data ["🗄️ Persistence Layer"]
        Prisma[Prisma ORM 5.22]
        PostgreSQL[(PostgreSQL Relational DB)]
    end

    UI <-->|HTTP / REST JSON| Security
    Security --> AuthGuard --> Router
    ChatClient <-->|WebSockets ws://| SocketServer
    Router <--> ContentFilter
    Router <--> Prisma
    SocketServer <--> Prisma
    Prisma <--> PostgreSQL
    Router <--> Cloudinary
```

---

## 🔄 Transaction & Escrow Protocol

The complete lifecycle of a secure campus deal:

```mermaid
sequenceDiagram
    autonumber
    actor Buyer as 🎓 Buyer (Student)
    actor Seller as 🎒 Seller (Student)
    participant API as ⚡ MUJMart Server
    participant DB as 🗄️ PostgreSQL / Escrow

    Buyer->>Seller: Browse listing & initiate negotiation chat
    Buyer->>Seller: Send offer via Socket.io Thread
    Seller->>Buyer: Counter-offer or Accept Offer
    Note over Buyer,Seller: Thread Status → "accepted"
    Buyer->>API: Create Transaction (status: pending_payment)
    API-->>Buyer: Return Seller's UPI QR Code
    Buyer->>API: Pay via UPI & submit UTR + Payment Screenshot
    API->>DB: Lock Funds in Escrow (status: escrow)
    API-->>Seller: 🔔 Notify: Payment verified. Please handoff item!
    Note over Buyer,Seller: 🤝 Physical item handoff on MUJ Campus
    Buyer->>API: Confirm Handover & Item Condition OK
    API->>DB: Status → ready_for_payout
    API->>Seller: Release payment to Seller's UPI ID (minus 5% margin)
    API->>DB: Mark Transaction Completed ✅
    API-->>Buyer: 🔔 Deal Complete! RepScore updated.
```

---

## 🧰 Tech Stack

### 🖥️ Frontend Application

| Layer | Technology | Version | Details |
|---|---|---|---|
| **Framework** | [Next.js](https://nextjs.org/) | 16 | App Router, Server Components & Static Optimization |
| **Library** | [React](https://react.dev/) | 19 | Concurrent UI rendering with Suspense |
| **Language** | [TypeScript](https://www.typescriptlang.org/) | 5 | Strict type safety across all components |
| **Styling** | [Tailwind CSS](https://tailwindcss.com/) | 4 | CSS variables & lightning-fast utility engine |
| **Realtime** | [Socket.io Client](https://socket.io/) | 4.8 | Bi-directional WebSocket communication |
| **QR Engine** | [qrcode.react](https://www.npmjs.com/package/qrcode.react) | Latest | Dynamic UPI QR code generation for payments |
| **Analytics** | [@vercel/analytics](https://vercel.com/analytics) | Latest | Real user monitoring & performance tracking |

### ⚙️ Backend API & Database

| Layer | Technology | Version | Details |
|---|---|---|---|
| **Runtime** | [Node.js](https://nodejs.org/) | 18+ | Fast V8 JavaScript runtime |
| **Framework** | [Express](https://expressjs.com/) | 4.21.2 | RESTful routing and API orchestration |
| **Language** | [TypeScript](https://www.typescriptlang.org/) | 5.7.2 | Typed controllers, models & route handlers |
| **ORM** | [Prisma](https://www.prisma.io/) | 5.22 | Type-safe queries, migrations, and schema modeling |
| **Database** | [PostgreSQL](https://www.postgresql.org/) | Latest | ACID-compliant relational data store |
| **WebSockets** | [Socket.io](https://socket.io/) | 4.8.1 | Room-based real-time chat & deal events |
| **Auth** | [JWT](https://jwt.io/) + [bcrypt](https://www.npmjs.com/package/bcrypt) | 9.0.2 / 5.1.1 | Stateless tokens & salt-hashed passwords (10 rounds) |
| **Media Storage** | [Cloudinary](https://cloudinary.com/) | 1.41.3 | Image optimization and secure document CDN |
| **Security** | [Helmet](https://helmetjs.github.io/) + CORS + Rate-Limit | 8.0.0 | Defense against XSS, brute-force & MIME attacks |
| **File Uploads** | [Multer](https://github.com/expressjs/multer) | 2.0.1 | Multipart form data handling for image uploads |
| **Testing** | [Jest](https://jestjs.io/) + [Supertest](https://github.com/ladjs/supertest) | 30.5 / 7.2.2 | Automated API integration and unit testing |
| **Dev Tools** | [ts-node-dev](https://github.com/wclr/ts-node-dev) | 2.0.0 | Hot-reload TypeScript dev server |

---

## 🗃️ Database Schema & Data Models

The Prisma relational model (`backend/prisma/schema.prisma`) powers all of MUJMart's data:

```mermaid
erDiagram
    User ||--o{ Listing : "creates (as seller)"
    User ||--o{ Thread : "participates (buyer or seller)"
    User ||--o{ Message : "sends"
    User ||--o{ Transaction : "engages in (buyer or seller)"
    User ||--o{ Dispute : "files as reporter"
    User ||--o{ Notification : "receives"
    User ||--o{ ProjectRequest : "requests or owns"

    Listing ||--o{ Thread : "has negotiation threads"
    Listing ||--o{ Transaction : "generates transactions"
    Listing ||--o{ ProjectRequest : "receives collaboration requests"

    Thread ||--o{ Message : "contains messages"
    Thread ||--o{ Dispute : "can have disputes"
```

### 📋 Key Models Reference

| Model | Primary Purpose | Key Fields |
|---|---|---|
| `User` | Student & Admin Accounts | `id`, `name`, `email`, `role`, `alias`, `upiId`, `upiQrUrl`, `repScore`, `dealCount`, `isBanned` |
| `Listing` | Marketplace Item Catalogue | `id`, `title`, `description`, `price`, `type`, `category`, `condition`, `images`, `status`, `expiresAt` |
| `Thread` | Negotiation Chat Room | `id`, `status` (*open/accepted/closed/rejected*), `listingId`, `buyerId`, `sellerId` |
| `Message` | Chat Messages | `id`, `threadId`, `senderId`, `content`, `isFiltered`, `createdAt` |
| `Transaction` | Escrow Financial Record | `id`, `amount`, `platformMargin` (5%), `status`, `utrNumber`, `paymentScreenshotUrl` |
| `Dispute` | Dispute Arbitration Cases | `id`, `threadId`, `reporterId`, `reason`, `status` (*open/resolved/dismissed*) |
| `Notification` | System & Deal Alerts | `id`, `userId`, `type`, `content`, `isRead`, `relatedId` |
| `ProjectRequest` | Student Task Collaborations | `id`, `listingId`, `requesterId`, `ownerId`, `status` |

---

## 🔌 API Reference

### 🔐 Authentication (`/api/auth`)

| Method | Endpoint | Access | Description |
|---|---|---|---|
| `POST` | `/api/auth/register` | Public | Register student with name, email, password, and campus alias |
| `POST` | `/api/auth/login` | Public | Authenticate user & return signed JWT token |
| `GET` | `/api/auth/me` | 🔒 Authenticated | Retrieve current user profile, stats, and UPI payout data |
| `PUT` | `/api/auth/profile` | 🔒 Authenticated | Update contact info, address, and UPI ID |
| `POST` | `/api/auth/upload-qr` | 🔒 Authenticated | Upload UPI QR image to Cloudinary |

### 📦 Marketplace Listings (`/api/listings`)

| Method | Endpoint | Access | Description |
|---|---|---|---|
| `GET` | `/api/listings` | Public | List active listings with search, category, type, and price filters |
| `GET` | `/api/listings/:id` | Public | Retrieve single listing detail with full seller info |
| `POST` | `/api/listings` | 🔒 Authenticated | Create new listing (supports multi-image Cloudinary upload) |
| `PUT` | `/api/listings/:id` | 🔒 Owner / Admin | Update listing information or price |
| `DELETE` | `/api/listings/:id` | 🔒 Owner / Admin | Soft-delete or remove listing |
| `GET` | `/api/listings/user/my` | 🔒 Authenticated | Get current user's active, sold, and expired listings |

### 💬 Negotiations & Chat (`/api/threads`)

| Method | Endpoint | Access | Description |
|---|---|---|---|
| `GET` | `/api/threads` | 🔒 Authenticated | Get all active negotiation threads for logged-in user |
| `POST` | `/api/threads` | 🔒 Authenticated | Initiate or open negotiation thread for a listing |
| `GET` | `/api/threads/:id` | 🔒 Participant | Fetch full message history of a thread |
| `PATCH` | `/api/threads/:id/status` | 🔒 Participant | Update negotiation status (`accepted`, `rejected`, `closed`) |
| `POST` | `/api/threads/:id/dispute` | 🔒 Participant | File formal dispute for admin moderator review |

### 💳 Escrow & Transactions (`/api/transactions`)

| Method | Endpoint | Access | Description |
|---|---|---|---|
| `GET` | `/api/transactions` | 🔒 Authenticated | Fetch buyer and seller transaction history |
| `POST` | `/api/transactions` | 🔒 Authenticated | Create transaction record upon accepted offer |
| `POST` | `/api/transactions/:id/pay` | 🔒 Buyer | Submit UTR reference number & payment receipt screenshot |
| `PATCH` | `/api/transactions/:id/status` | 🔒 Buyer/Seller/Admin | Progress escrow status (confirm handoff, release payout) |

### 🤝 Project Requests (`/api/requests`)

| Method | Endpoint | Access | Description |
|---|---|---|---|
| `GET` | `/api/requests` | 🔒 Authenticated | Fetch incoming & outgoing task/collaboration applications |
| `POST` | `/api/requests` | 🔒 Authenticated | Submit collaboration request for a project listing |
| `PATCH` | `/api/requests/:id` | 🔒 Owner | Accept or reject incoming collaboration application |

### 🔔 Notifications (`/api/notifications`)

| Method | Endpoint | Access | Description |
|---|---|---|---|
| `GET` | `/api/notifications` | 🔒 Authenticated | Fetch all unread and read notifications for the user |
| `PATCH` | `/api/notifications/:id/read` | 🔒 Authenticated | Mark a notification as read |
| `PATCH` | `/api/notifications/read-all` | 🔒 Authenticated | Mark all notifications as read |

### 👑 Admin Management (`/api/admin`)

| Method | Endpoint | Access | Description |
|---|---|---|---|
| `GET` | `/api/admin/metrics` | 🛡️ Admin Only | Get system stats — users, transaction volume, margins, disputes |
| `GET` | `/api/admin/users` | 🛡️ Admin Only | Manage all student users and inspect profiles |
| `PATCH` | `/api/admin/users/:id/ban` | 🛡️ Admin Only | Ban or unban a user from the marketplace |
| `GET` | `/api/admin/disputes` | 🛡️ Admin Only | View all open dispute claims with evidence |
| `PATCH` | `/api/admin/disputes/:id` | 🛡️ Admin Only | Adjudicate dispute (*resolved* or *dismissed*) |
| `GET` | `/api/admin/transactions` | 🛡️ Admin Only | Audit all platform transactions and payout states |

---

## ⚡ Quickstart Guide

### Prerequisites

Ensure the following are installed on your machine:

| Tool | Version | Download |
|---|---|---|
| **Node.js** | v18.0.0+ | [nodejs.org](https://nodejs.org/) |
| **npm** | v9.0.0+ | Bundled with Node.js |
| **PostgreSQL** | Latest | [postgresql.org](https://www.postgresql.org/) or use [Neon](https://neon.tech/) / [Supabase](https://supabase.com/) / [Render](https://render.com/) |
| **Git** | Latest | [git-scm.com](https://git-scm.com/) |

> 💡 **Tip**: No PostgreSQL locally? Use a free cloud provider like [Neon.tech](https://neon.tech) and just paste the connection string!

---

### Step 1 — Clone the Repository

```bash
git clone https://github.com/abhinendrasinghDS/mujmart---in-.git
cd mujmart---in-
```

---

### Step 2 — One-Command Setup

Install all dependencies across root, frontend, and backend with a single command:

```bash
npm run install-all
```

> This installs packages for: root monorepo, `/frontend` (Next.js), and `/backend` (Express + Prisma).

---

### Step 3 — Configure Environment Variables

Navigate to the backend directory and create your `.env` file:

```bash
cd MujMart-main/backend
cp .env.example .env
```

Open `backend/.env` and fill in your credentials:

```env
# ─── Server Config ────────────────────────────────────
PORT=4000
NODE_ENV=development

# ─── CORS ─────────────────────────────────────────────
FRONTEND_URL=http://localhost:3000

# ─── PostgreSQL Database ──────────────────────────────
# Local example:
DATABASE_URL="postgresql://postgres:yourpassword@localhost:5432/mujmart?schema=public"
# Cloud example (Neon/Supabase):
# DATABASE_URL="postgresql://user:pass@host/dbname?sslmode=require"

# ─── JWT Security ─────────────────────────────────────
# Use a long, random string (32+ characters) in production!
JWT_SECRET=super_secret_jwt_key_mujmart_2026_change_in_prod

# ─── Cloudinary (Optional for local dev, required in production) ──
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
```

---

### Step 4 — Database Setup & Seeding

From the **repository root**, run the complete database setup:

```bash
npm run db:setup
```

This single command will:
1. ✅ Generate Prisma Client
2. ✅ Apply database migrations
3. ✅ Seed campus mock users, listings & demo transactions

> **Or run steps individually:**
> ```bash
> npm run db:generate   # Generate Prisma Client typings
> npm run db:migrate    # Apply all pending migrations
> npm run db:seed       # Seed mock campus data
> ```

> 💡 **Pro Tip**: Inspect your database visually anytime:
> ```bash
> npm run db:studio
> # Opens Prisma Studio at http://localhost:5555
> ```

---

### Step 5 — Launch Development Servers

Start **both Frontend and Backend** concurrently with a single command:

```bash
npm run dev
```

| Service | URL | Description |
|---|---|---|
| 🌐 **Next.js Frontend** | [http://localhost:3000](http://localhost:3000) | Campus marketplace UI |
| ⚡ **Express REST API** | [http://localhost:4000](http://localhost:4000) | Backend API server |
| 🔌 **Socket.io** | `ws://localhost:4000` | Real-time chat WebSocket |
| 📊 **Prisma Studio** | [http://localhost:5555](http://localhost:5555) | Visual DB explorer (run `npm run db:studio`) |

**You're live!** Open [http://localhost:3000](http://localhost:3000) to explore MUJMart. 🎉

---

## 📂 Project Structure

```
mujmart---in-/
└── MujMart-main/
    ├── frontend/                         # 🖥️ Next.js 16 Application
    │   ├── public/                       # Static assets (logo, banners, QR, icons)
    │   └── src/
    │       ├── app/                      # App Router Pages (file-based routing)
    │       │   ├── admin/                # 👑 Admin dashboard (users, disputes, metrics)
    │       │   │   ├── disputes/         # Dispute review & arbitration
    │       │   │   ├── escrow/           # Escrow & payout management
    │       │   │   ├── listings/         # Platform-wide listing moderation
    │       │   │   ├── margins/          # Revenue & margin tracking
    │       │   │   ├── rent/             # Rental management
    │       │   │   ├── settings/         # Admin platform settings
    │       │   │   └── users/            # User management & bans
    │       │   ├── cart/                 # 🛒 Saved items & checkout flow
    │       │   ├── chat/[threadId]/      # 💬 Realtime Socket.io negotiation room
    │       │   ├── help/                 # ❓ Help Center, FAQ & WhatsApp support
    │       │   ├── listing/[id]/         # 📦 Listing detail view & offer modal
    │       │   ├── login/                # 🔐 Campus student login & registration
    │       │   ├── my-listings/          # 📋 User's personal inventory management
    │       │   ├── notifications/        # 🔔 Real-time notification center
    │       │   ├── post/                 # ✏️ Create listing wizard (sell/rent/share/task)
    │       │   ├── profile/[id]/         # 👤 Public user profile, UPI details & rep score
    │       │   ├── report-issue/         # 🚨 Dispute & bug ticket filing with uploads
    │       │   ├── search/               # 🔍 Category search & faceted filters
    │       │   ├── settings/             # ⚙️ Account preferences & security
    │       │   ├── task/[id]/            # 🤝 Campus task / project collaboration detail
    │       │   ├── sitemap.ts            # SEO sitemap generation
    │       │   ├── layout.tsx            # Global layout — persistent Navbar & Footer
    │       │   └── page.tsx              # 🏠 Hero homepage with featured listings
    │       ├── components/               # Reusable UI components
    │       │   ├── admin/                # Admin-specific components
    │       │   ├── auth/                 # Login & auth modals
    │       │   ├── marketplace/          # Listing cards, search bar, hero banner
    │       │   └── ui/                   # Generic UI primitives (badges, tags, avatars)
    │       └── lib/                      # Utilities, API clients & React contexts
    │           ├── AuthContext.tsx        # Global authentication state
    │           ├── CartContext.tsx        # Shopping cart state management
    │           ├── DemoContext.tsx        # Demo mode data context
    │           ├── api.ts                 # Typed API client functions
    │           ├── firebase.ts            # Firebase client setup
    │           └── mockData.ts            # Local mock data for demo mode
    │
    ├── backend/                          # ⚙️ Express + TypeScript Server
    │   ├── prisma/
    │   │   ├── schema.prisma             # 🗄️ Database models & relationships
    │   │   └── seed.ts                   # 🌱 Seed data: campus categories & demo users
    │   └── src/
    │       ├── middleware/               # Express middleware
    │       │   ├── auth.ts               # JWT verification & role guards
    │       │   └── contentFilter.ts      # contentGuard: blocks contact leakage in chat
    │       ├── routes/                   # REST API route handlers
    │       │   ├── admin.ts              # Metrics, user bans, dispute resolution
    │       │   ├── auth.ts               # Registration, login, profile, UPI QR
    │       │   ├── listings.ts           # Listing CRUD, search & filters
    │       │   ├── notifications.ts      # Notification read/unread tracking
    │       │   ├── requests.ts           # Collaboration request workflows
    │       │   ├── threads.ts            # Chat threads, messages & content filter
    │       │   └── transactions.ts       # Escrow logic, UTR verification & payouts
    │       ├── socket/
    │       │   └── chat.ts               # 🔌 Socket.io real-time event handler
    │       ├── tests/
    │       │   └── api.test.ts           # 🧪 Jest + Supertest integration tests
    │       └── index.ts                  # 🚀 Server bootstrap & Socket.io attachment
    │
    ├── package.json                      # Root monorepo scripts
    ├── .gitignore                        # Git ignore rules
    └── README.md                         # 📖 This documentation
```

---

## 📜 All Available Scripts

Run all commands from the **repository root** (`MujMart-main/`):

| Command | Action |
|---|---|
| `npm run dev` | 🚀 Start **both** Frontend (port 3000) and Backend (port 4000) concurrently |
| `npm run dev:frontend` | Start only the Next.js frontend |
| `npm run dev:backend` | Start only the Express API server |
| `npm run setup` | 🔧 Full initial setup: install all packages + complete DB setup |
| `npm run install-all` | 📦 Install all deps in root, frontend, and backend |
| `npm run build` | 🏗️ Compile frontend for production |
| `npm run build:backend` | 🏗️ Compile backend TypeScript to `dist/` |
| `npm run lint` | 🔍 Run ESLint over frontend code |
| `npm run db:setup` | 🗄️ Generate client + apply migrations + seed database |
| `npm run db:generate` | Regenerate Prisma Client typings |
| `npm run db:migrate` | Run pending Prisma migrations |
| `npm run db:seed` | 🌱 Populate sample campus data into PostgreSQL |
| `npm run db:reset` | ⚠️ Wipe database, re-apply migrations & reseed from scratch |
| `npm run db:studio` | 📊 Open Prisma Studio visual DB explorer at port 5555 |

---

## 🧪 Testing

The backend includes automated integration tests powered by **Jest** and **Supertest**:

```bash
# Navigate to backend directory
cd MujMart-main/backend

# Run the full test suite
npm test
```

Tests cover:
- ✅ User registration & authentication flows
- ✅ Listing creation, search, and retrieval
- ✅ Thread creation and status transitions
- ✅ Transaction escrow state machine
- ✅ Admin-protected route access control

---

## 🛡️ Security & Campus Integrity

MUJMart implements **multi-layered security controls**:

| Layer | Mechanism | Details |
|---|---|---|
| **Authentication** | JWT (HMAC-SHA256) | Stateless tokens with configurable expiry |
| **Password Safety** | `bcrypt` | 10 salt rounds, never stored in plaintext |
| **HTTP Security Headers** | `helmet` | Protects against XSS, clickjacking, MIME-sniffing |
| **Abuse Mitigation** | `express-rate-limit` | Prevents brute-force logins and spam listing creation |
| **Content Filtering** | `contentGuard` middleware | Server-side regex redacts phone numbers & handles in chat |
| **CORS Policy** | Strict origin whitelist | Only allows requests from configured `FRONTEND_URL` |
| **Dispute Redressal** | Admin Tribunal | Any user can escalate a chat thread to admin review |

---

## 🗺️ Roadmap & Upcoming Enhancements

| Status | Feature | Description |
|---|---|---|
| 🔲 Planned | **Campus SSO Integration** | Direct Manipal University Jaipur Microsoft/Google OAuth login |
| 🔲 Planned | **AI-Powered Fair Price Estimator** | Suggests fair prices based on historical campus deal data |
| 🔲 Planned | **Hostel Room Delivery Network** | Peer-to-peer student courier system for intra-campus delivery |
| 🔲 Planned | **Direct UPI Deep-Linking** | One-tap intent payments via GPay, PhonePe, and Paytm |
| 🔲 Planned | **Progressive Web App (PWA)** | Offline browsing and native push notifications on mobile |
| 🔲 Planned | **Semester Book Exchange** | Dedicated semester-start bulk buy/sell of textbooks |
| 🔲 Planned | **Hostel Lost & Found Board** | Dedicated category for reporting and finding lost items |

---

## 🤝 Contributing

Contributions from the MUJ student and open-source developer community are warmly welcome!

1. **Fork** this repository
2. **Create your Feature Branch**:
   ```bash
   git checkout -b feature/your-amazing-feature
   ```
3. **Commit your changes** (follow conventional commits):
   ```bash
   git commit -m "feat: add amazing campus feature"
   ```
4. **Push to your branch**:
   ```bash
   git push origin feature/your-amazing-feature
   ```
5. **Open a Pull Request** on GitHub with a clear description of your changes.

### Commit Message Convention

| Prefix | When to Use |
|---|---|
| `feat:` | New feature added |
| `fix:` | Bug fix |
| `docs:` | Documentation changes only |
| `style:` | Code formatting (no logic change) |
| `refactor:` | Code restructuring without feature change |
| `test:` | Adding or fixing tests |
| `chore:` | Maintenance tasks, dependency updates |

---

## 📄 License

This project is licensed under the **MIT License** — free to use, modify, and distribute with attribution.

---

## 🙏 Acknowledgements

- **Manipal University Jaipur** — The inspiration and community behind this platform.
- **Prisma Team** — For the incredible TypeScript-first ORM.
- **Vercel** — For seamless Next.js deployment and analytics.
- **Socket.io** — For making real-time negotiation effortless.
- **Cloudinary** — For reliable media storage and transformation.

---

<div align="center">

  ### 👨‍💻 Developed with ❤️ for the MUJ Community

  *Empowering students at Manipal University Jaipur through modern open-source technology.*

  <br />

  [![GitHub Stars](https://img.shields.io/github/stars/abhinendrasinghDS/mujmart---in-?style=social)](https://github.com/abhinendrasinghDS/mujmart---in-)
  &nbsp;&nbsp;&nbsp;&nbsp;
  [![GitHub Follow](https://img.shields.io/github/followers/abhinendrasinghDS?label=Follow%20abhinendrasinghDS&style=social)](https://github.com/abhinendrasinghDS)

  <br />

  **[⬆ Back to Top](#-mujmart)**

</div>
