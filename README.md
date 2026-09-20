# 🛒 NexaMart 🚀

![Demo App](/frontend/public/HexaMart_Preview_Image.png)

---

## 🧩 Tech Stack

NexaMart is a full-stack commerce platform built for modern storefront operations, customer support, and admin product management.

### Frontend
- React 19 + Vite
- TanStack Query for data fetching and cache management
- Tailwind CSS + DaisyUI for UI styling
- React Router for client-side navigation
- Zustand for lightweight cart state management

### Backend
- Node.js + Express.js
- TypeScript for type-safe server logic
- Drizzle ORM with PostgreSQL
- Clerk for authentication and user identity
- Polar for checkout and payment orchestration

### Real-time & Media
- Stream Chat and Stream Video for support conversations and live sessions
- ImageKit for image optimization and delivery
- Sentry for monitoring, error tracking, and performance insights

### Operational Features
- Admin product management dashboard
- Product catalog and cart workflows
- Order lifecycle tracking
- Secure webhook integrations
- Structured logging and deployment-ready app architecture

---

## ✨ Platform Highlights

- Multi-step ecommerce flow from catalog browsing to checkout and order tracking
- Secure customer authentication with role-aware admin access
- Real-time customer support chat with reactions, typing indicators, and thread-based conversations
- Video-enabled support workflows for order assistance
- Media optimization and branded image overlays for storefront content
- Production-oriented monitoring, logging, and error handling

---

## ▶️ How to Run

### 1) Install dependencies

```bash
cd backend && npm install
cd ../frontend && npm install
```

### 2) Configure environment variables

Create a `.env` file in the backend and frontend folders using the values below in the Environment Variables section.

### 3) Start the backend

```bash
cd backend
npm run dev
```

The API server will run on the port defined in `PORT` (for example `http://localhost:3000`).

### 4) Start the frontend

```bash
cd frontend
npm run dev -- --host 0.0.0.0
```

The app will typically open at:

```bash
http://localhost:5173
```

---

## 🧪 Environment Variables

### Backend (`/backend`)

```bash
PORT=<your_port>
NODE_ENV=<development_or_production>

DATABASE_URL=<your_postgresql_connection_string>

CLERK_PUBLISHABLE_KEY=<your_clerk_publishable_key>
CLERK_SECRET_KEY=<your_clerk_secret_key>
CLERK_WEBHOOK_SECRET=<your_clerk_webhook_secret>

SENTRY_DSN=<your_sentry_dsn>

STREAM_API_KEY=<your_stream_api_key>
STREAM_API_SECRET=<your_stream_api_secret>

IMAGEKIT_PUBLIC_KEY=<your_imagekit_public_key>
IMAGEKIT_PRIVATE_KEY=<your_imagekit_private_key>
IMAGEKIT_URL_ENDPOINT=<your_imagekit_url_endpoint>

FRONTEND_URL=<your_frontend_url>

POLAR_ACCESS_TOKEN=<your_polar_access_token>
POLAR_WEBHOOK_SECRET=<your_polar_webhook_secret>
POLAR_API_BASE=<your_polar_api_base_url>

POLAR_CHECKOUT_PRODUCT_ID=<your_product_id>
```

### Frontend (`/frontend`)

```bash
VITE_CLERK_PUBLISHABLE_KEY=<your_clerk_publishable_key>
VITE_SENTRY_DSN=<your_sentry_dsn>
VITE_API_URL=<your_backend_api_url>
```
