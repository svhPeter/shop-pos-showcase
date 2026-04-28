<div align="center">

# 🏪 ShopPOS

### The Complete Multi-Tenant POS & Shop Management SaaS

**Production-ready · Battle-tested · Ready to deploy**

A full-featured Point of Sale and shop management system built for cafes, retail stores, and multi-location businesses. Multi-tenant architecture means **one deployment serves unlimited shops** — perfect for SaaS founders who want to launch fast.

[![Live Demo](https://img.shields.io/badge/🚀_Live_Demo-shop--pos--sand.vercel.app-000?style=for-the-badge)](https://shop-pos-sand.vercel.app/)
[![Available for License](https://img.shields.io/badge/Available_for_License-22c55e?style=for-the-badge)](https://www.aibuddy.design)
[![One-Time Purchase](https://img.shields.io/badge/One--Time_Purchase-3b82f6?style=for-the-badge)](https://www.aibuddy.design)

[**🌐 Live Demo**](https://shop-pos-sand.vercel.app/) · [**💰 Buy / License**](https://www.aibuddy.design) · [**📧 Contact**](https://www.aibuddy.design)

</div>

---

## 🎯 Who This Is For

> **SaaS founders, agencies, and entrepreneurs** who want to launch a POS or shop management product **in days, not months.**

- ✅ You want to start a SaaS business serving cafes, retail, or small shops
- ✅ You're an agency that wants to white-label and resell to multiple clients
- ✅ You need a production-ready codebase you can fork, brand, and ship
- ✅ You don't want to spend 6+ months building auth, multi-tenancy, billing, and reports from scratch

**Skip the hard parts. Get a working product. Customize and launch.**

---

## 🖼️ Screenshots

> _Screenshots placeholder — drop images in `/screenshots` folder and update paths_

| Dashboard | POS Sale Flow | Inventory |
|-----------|---------------|-----------|
| ![Dashboard](./screenshots/dashboard.png) | ![POS](./screenshots/pos.png) | ![Inventory](./screenshots/inventory.png) |

| Reports | Multi-Tenant Admin | Staff & Shifts |
|---------|-------------------|----------------|
| ![Reports](./screenshots/reports.png) | ![Admin](./screenshots/admin.png) | ![Staff](./screenshots/staff.png) |

---

## ⚡ Live Demo

**👉 [shop-pos-sand.vercel.app](https://shop-pos-sand.vercel.app/)**

Try it live — explore the landing page, features, pricing, and login flow. Two seeded demo tenants are available (retail + coffee shop) so you can see how multi-tenancy actually works.

---

## ✨ What's Inside

### 🏢 Multi-Tenant Architecture
- **Data isolation** by `tenantId` — deploy once, serve unlimited shops
- **Platform admin panel** — create new tenants, hand over to buyers
- **Role-based access control** — owner, staff, platform admin

### 🛒 Point of Sale
- Fast checkout with **barcode scanning** support
- Cart, multiple payment methods, instant receipts
- **Atomic stock deduction** — no overselling, ever
- POS-friendly endpoint: `GET /api/products/lookup?barcode=...`

### 📦 Inventory Management
- Products, categories, stock levels, restock workflows
- Low-stock alerts with **realtime notifications + sound**
- Stock movements & adjustment history
- Cost price tracking + margin visibility

### 🚚 Suppliers & Purchases
- Full supplier CRUD, link products to suppliers
- Record purchases with cost, quantity, supplier reference
- Inventory valuation reporting

### 💰 Expenses & Accounting
- Categorized expense tracking
- **QuickBooks CSV export** + generic CSV (sales/expenses)
- Tax reports, daily revenue, expenses by category

### 👥 Staff & Shifts
- Staff CRUD, shift scheduling
- Check-in / check-out, hours-worked tracking

### 📊 Reports & Analytics
- Financial summary, top products, low stock
- Daily revenue, expenses by category, tax report
- Inventory valuation

### 🔌 Integrations
- **Outbound webhooks** for sale / purchase / inventory / expense events
- Test webhooks from the UI
- Accounting CSV exports for QuickBooks & generic systems

### ⚡ Realtime
- **Server-Sent Events (SSE)** — live dashboard, sales, inventory updates
- Polling fallback (30s) when SSE disconnects
- Notification bell with sound + popup for low-stock alerts

### 🔒 Security & Reliability
- Cookie-based session authentication, bcrypt hashing
- HMAC-signed session tokens
- Forgot / reset password (Resend integration optional)
- **Audit logging** on all write operations
- Health check endpoint: `GET /api/health`
- Consistent error format: `{ error, code, details? }`
- Paginated list endpoints: `{ data, meta }`

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| **Framework** | Next.js 16 (App Router + API Routes) |
| **Language** | TypeScript 5 |
| **Database** | PostgreSQL (Neon Serverless) |
| **ORM** | Prisma 7 |
| **Validation** | Zod 4 |
| **Auth** | Cookie sessions + bcrypt |
| **Deployment** | Vercel (recommended) or self-hosted Docker |
| **Realtime** | Server-Sent Events (SSE) |

**Modern, production-grade, and proven at scale.**

---

## 🏗️ Architecture Highlights
