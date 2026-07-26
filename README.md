<h1 align="center">Allah Nawaz</h1>
<h3 align="center">Full Stack Developer · MERN & Next.js</h3>

<p align="center">
  I build and ship production web applications — eCommerce platforms, real-time systems, and multi-tenant SaaS.
</p>

<p align="center">
  <a href="https://allahnawaz-dev.vercel.app/"><img src="https://img.shields.io/badge/Portfolio-1F3864?style=flat-square&logo=vercel&logoColor=white" alt="Portfolio" /></a>
  <a href="https://www.linkedin.com/in/allahnawaz-dev/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:nawaz51412@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
</p>

---

### About

- 🏢 Building at **Algotix AI** — versioned REST APIs, RBAC auth, and real-time notification workflows
- 🔭 Focused on **backend architecture, multi-tenant SaaS, and real-time systems**
- 🌱 Going deeper on **system design, TypeScript at scale, and DevOps fundamentals**
- 💬 Ask me about **REST API design, RBAC, Socket.IO, Next.js SSR, or Prisma schema modeling**
- 📬 Reach me at **nawaz51412@gmail.com**

---

## Tech Stack

**Frontend**

![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Redux Toolkit](https://img.shields.io/badge/Redux%20Toolkit-764ABC?style=flat-square&logo=redux&logoColor=white)
![RTK Query](https://img.shields.io/badge/RTK%20Query-764ABC?style=flat-square&logo=redux&logoColor=white)
![Zustand](https://img.shields.io/badge/Zustand-433E38?style=flat-square&logo=react&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)

> Component composition patterns · State architecture design · Reusable UI systems · SSR & Core Web Vitals optimization · Technical SEO

**Backend**

![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white)
![Socket.IO](https://img.shields.io/badge/Socket.IO-010101?style=flat-square&logo=socketdotio&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white)
![Stripe](https://img.shields.io/badge/Stripe-635BFF?style=flat-square&logo=stripe&logoColor=white)
![Twilio](https://img.shields.io/badge/Twilio-F22F46?style=flat-square&logo=twilio&logoColor=white)

> Modular backend architecture · RESTful API design & versioning · Role-based access control · Middleware layering · Controller–service separation · Error handling strategy

**Database & Storage**

![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Mongoose](https://img.shields.io/badge/Mongoose-880000?style=flat-square&logo=mongodb&logoColor=white)
![AWS S3](https://img.shields.io/badge/AWS%20S3-569A31?style=flat-square&logo=amazons3&logoColor=white)

> Schema modeling · Indexing & query optimization · Multi-tenant data isolation · Transactional integrity under concurrent writes

**Deployment & Workflow**

![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white)
![PM2](https://img.shields.io/badge/PM2-2B037A?style=flat-square&logo=pm2&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white)

> VPS deployment with Nginx reverse proxy & PM2 · SSL configuration · Environment-based config · Continuous deployment from GitHub

---

## Featured Projects

### 🌿 Herbal Mart PK — Production eCommerce Platform
[![Live](https://img.shields.io/badge/Live-herbalmart.com.pk-1F3864?style=flat-square)](https://herbalmart.com.pk/)

A production full-stack storefront serving live customer traffic, covering the complete funnel from catalog to checkout.

- Technical SEO layer: dynamic per-page metadata, JSON-LD structured data, generated `sitemap.xml` and `robots.txt` — product pages crawlable and eligible for rich results
- Role-protected admin dashboard for product, category, inventory, and order management with full CRUD
- JWT auth over HTTP-only cookies, validated REST APIs, and automated transactional email via NodeMailer

`Next.js (App Router)` · `React` · `Node.js` · `Express` · `MongoDB` · `Redux Toolkit` · `RTK Query` · `Tailwind CSS`

---

### 🚕 Aleet — Car Booking & Ride Management
[![Live](https://img.shields.io/badge/Live-aleet.app-1F3864?style=flat-square)](https://www.aleet.app/)

Ride-booking platform supporting membership, hourly, and multi-day packages.

- Real-time trip tracking over Socket.IO with instant driver payouts through Stripe
- AWS S3 for secure document and image storage; Twilio for automated SMS booking confirmations
- RBAC separating guest, operator, and driver permissions behind JWT + HTTP-only cookies

`Next.js` · `Node.js` · `PostgreSQL` · `Stripe` · `AWS S3` · `Twilio` · `Socket.IO`

---

### 🏢 Check Point — Multi-Tenant SaaS Platform

Multi-tenant architecture with organization-level data isolation and secure tenant onboarding.

- Cross-tenant data exposure prevented by design at the schema and query layer
- Prisma-backed models enforcing strict type safety and referential integrity across tenant boundaries
- Scalable role and permission system supporting distinct access hierarchies per organization

`Node.js` · `Express` · `PostgreSQL` · `Prisma ORM` · `RBAC`

---

### 🏥 Clinic Queue System — Real-Time Workflow Engine
[![Live](https://img.shields.io/badge/Live-Demo-1F3864?style=flat-square)](https://clinic-queue-frontend.vercel.app/)

Patient queue engine built for correctness under concurrent updates.

- Sub-second queue state transitions backed by PostgreSQL transactions for data integrity
- Role-based dashboards for doctors, receptionists, and admins, synchronized live via Socket.IO

`React` · `Node.js` · `Express` · `PostgreSQL` · `Socket.IO`

---

### 🛒 MyHerb.pk — Full-Stack eCommerce Application
[![Live](https://img.shields.io/badge/Live-my--herb--pk.vercel.app-1F3864?style=flat-square)](https://my-herb-pk.vercel.app/)

Modern storefront with dynamic product and category routing and server-rendered listing pages.

- Redux Toolkit + RTK Query for client state and server cache — no duplicate API calls, consistent cart state across routes
- Stateless JWT auth over secure REST APIs with protected customer and admin route groups
- SEO-friendly markup and crawlable URLs, image optimization, and route-level code splitting

`Next.js` · `React` · `Node.js` · `Express` · `MongoDB` · `Redux Toolkit` · `RTK Query` · `Tailwind CSS`

---

### 🚚 Allogo — Logistics & Ride-Booking Platform
[![Live](https://img.shields.io/badge/Live-Demo-1F3864?style=flat-square)](https://ailogo-gamma.vercel.app/)

Real-time logistics platform with live ride updates over Socket.IO, driver onboarding flows, and role-based access for drivers and dispatchers.

`React` · `Node.js` · `Express` · `MongoDB` · `Socket.IO` · `JWT` · `RBAC`

---

### 🔗 Smart Outreach — Internal Automation Tool

LinkedIn outreach automation with multi-account linking, campaign sequencing, and personalized connection-request workflows. Lead extraction from Sales Navigator feeding a backend pipeline that tracks campaign engagement end to end.

`Node.js` · `Express` · `MongoDB` · `REST APIs` · `Puppeteer`

---

## GitHub Stats

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=AN-code07&show_icons=true&theme=tokyonight&hide_border=true&rank_icon=github" alt="GitHub stats" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=AN-code07&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" alt="Top languages" />
</p>

---

<p align="center">
  <a href="https://allahnawaz-dev.vercel.app/">Portfolio</a> ·
  <a href="https://www.linkedin.com/in/allahnawaz-dev/">LinkedIn</a> ·
  <a href="mailto:nawaz51412@gmail.com">nawaz51412@gmail.com</a>
</p>
