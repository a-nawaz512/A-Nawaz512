<h1 align="center">Allah Nawaz</h1>
<h3 align="center">Full Stack Developer · MERN & Next.js</h3>

<p align="center">
  I build and ship production web applications — eCommerce platforms, real-time systems, and multi-tenant SaaS.
</p>

<p align="center">
  <a href="https://allahnawaz-dev.vercel.app/"><img src="https://img.shields.io/badge/Portfolio-1F3864?style=for-the-badge&logo=vercel&logoColor=white" alt="Portfolio" /></a>
  <a href="https://www.linkedin.com/in/allahnawaz-dev/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:nawaz51412@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
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

<p align="left">
  <img src="https://skillicons.dev/icons?i=react,nextjs,ts,js,redux,tailwind,html,css&theme=dark" height="60" alt="Frontend stack" />
</p>

**Backend**

<p align="left">
  <img src="https://skillicons.dev/icons?i=nodejs,express,prisma,nginx&theme=dark" height="60" alt="Backend stack" />
</p>

**Database & Storage**

<p align="left">
  <img src="https://skillicons.dev/icons?i=mongodb,postgres,aws&theme=dark" height="60" alt="Database stack" />
</p>

**Deployment & Tooling**

<p align="left">
  <img src="https://skillicons.dev/icons?i=vercel,linux,git,github,postman,docker,figma,vscode&theme=dark" height="60" alt="Tooling" />
</p>

<sub>**Also working with:** Socket.IO · RTK Query · Zustand · Mongoose · Stripe · Twilio · NodeMailer · PM2 · Puppeteer</sub>

---

## How I Build

**Request lifecycle** — middleware layering and controller–service separation, so business logic stays testable and transport concerns stay at the edge.

```mermaid
flowchart LR
    A["Client<br/>Next.js · React<br/>RTK Query"] --> B["Express Router<br/>versioned /api/v1"]
    B --> C["Middleware<br/>JWT · RBAC · Validation"]
    C --> D["Controller<br/>request/response only"]
    D --> E["Service Layer<br/>business logic"]
    E --> F[("MongoDB<br/>PostgreSQL")]
    E --> G["AWS S3<br/>object storage"]
    E --> H["Stripe · Twilio<br/>NodeMailer"]
    E -.->|domain events| I["Socket.IO"]
    I -.->|live push| A

    classDef c fill:#1F3864,stroke:#0d1b33,color:#ffffff
    classDef d fill:#2D6A4F,stroke:#1b4332,color:#ffffff
    classDef e fill:#6A3D9A,stroke:#432066,color:#ffffff
    class A,B,C,D,E c
    class F,G d
    class H,I e
```

**Authentication & role-based access** — the path every protected request takes, including why a request gets a 401 versus a 403 and where tenant scoping is applied.

```mermaid
sequenceDiagram
    participant U as Client
    participant A as Auth Middleware
    participant R as RBAC Guard
    participant C as Controller
    participant DB as Database

    U->>A: Request + HTTP-only cookie
    A->>A: Verify JWT signature & expiry
    alt Invalid or expired token
        A-->>U: 401 Unauthorized
    else Valid
        A->>R: Attach user identity + role
        R->>R: Check role against route policy
        alt Role not permitted
            R-->>U: 403 Forbidden
        else Authorized
            R->>C: Proceed
            C->>DB: Query scoped to tenant / owner
            DB-->>U: 200 Response
        end
    end
```

**Multi-tenant data isolation** — how tenant context is resolved and enforced before any query reaches shared storage.

```mermaid
flowchart TD
    R["Request<br/>+ tenant context"] --> M{"Tenant<br/>resolver"}
    M -->|org_id: A| QA["Prisma query<br/>scoped to Org A"]
    M -->|org_id: B| QB["Prisma query<br/>scoped to Org B"]
    QA --> DB[("Shared PostgreSQL<br/>row-level isolation")]
    QB --> DB
    M -->|no valid tenant| X["403 — reject"]

    classDef a fill:#1F3864,stroke:#0d1b33,color:#ffffff
    classDef b fill:#2D6A4F,stroke:#1b4332,color:#ffffff
    classDef c fill:#8B2635,stroke:#5c1922,color:#ffffff
    class R,M a
    class QA,QB,DB b
    class X c
```

---

## Projects

```mermaid
flowchart LR
    EC["eCommerce"] --> HM["Herbal Mart PK"]
    EC --> MH["MyHerb.pk"]
    RT["Real-Time Systems"] --> AL["Aleet"]
    RT --> CQ["Clinic Queue"]
    RT --> AG["Allogo"]
    SA["Multi-Tenant SaaS"] --> CP["Check Point"]
    AU["Automation"] --> SO["Smart Outreach"]

    classDef dom fill:#1F3864,stroke:#0d1b33,color:#ffffff
    classDef prj fill:#2D6A4F,stroke:#1b4332,color:#ffffff
    class EC,RT,SA,AU dom
    class HM,MH,AL,CQ,AG,CP,SO prj
```

| Project | Domain | Stack | Live |
|---|---|---|---|
| **Herbal Mart PK** | Production eCommerce | Next.js · Node.js · MongoDB · RTK Query · Tailwind | [herbalmart.com.pk](https://herbalmart.com.pk/) |
| **Aleet** | Ride booking & payouts | Next.js · PostgreSQL · Stripe · AWS S3 · Twilio · Socket.IO | [aleet.app](https://www.aleet.app/) |
| **MyHerb.pk** | Full-stack eCommerce | Next.js · Node.js · MongoDB · Redux Toolkit · Tailwind | [my-herb-pk.vercel.app](https://my-herb-pk.vercel.app/) |
| **Clinic Queue** | Real-time workflow engine | React · Node.js · PostgreSQL · Socket.IO | [Demo](https://clinic-queue-frontend.vercel.app/) |
| **Allogo** | Logistics & ride booking | React · Node.js · MongoDB · Socket.IO · RBAC | [Demo](https://ailogo-gamma.vercel.app/) |
| **Check Point** | Multi-tenant SaaS | Node.js · PostgreSQL · Prisma ORM · RBAC | — |
| **Smart Outreach** | Internal automation | Node.js · MongoDB · REST APIs · Puppeteer | — |

---

## Engineering Journey

```mermaid
timeline
    title From first commit to production systems
    2024 : Joined Codes Thinker
         : Next.js + Tailwind, SSR performance work
    2025 : Reusable React component library
         : PostgreSQL, JWT and RBAC hardening
    2026 : Joined Algotix AI
         : Prisma, versioned REST APIs, Socket.IO real-time
```

---

## GitHub Stats

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=AN-code07&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true&rank_icon=github" alt="GitHub stats" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=AN-code07&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" alt="Top languages" />
</p>

---

<p align="center">
  <a href="https://allahnawaz-dev.vercel.app/">Portfolio</a> ·
  <a href="https://www.linkedin.com/in/allahnawaz-dev/">LinkedIn</a> ·
  <a href="mailto:nawaz51412@gmail.com">nawaz51412@gmail.com</a>
</p>
