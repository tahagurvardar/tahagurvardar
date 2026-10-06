<h1 align="center">Hi, I'm Taha Gürvardar 👋</h1>

<h3 align="center">
Computer Engineering Student · Systems & Backend Engineer · Full-Stack Developer
</h3>

<p align="center">
I build distributed systems, real-time desktop software, and full-stack products with a focus on correctness, fault tolerance, concurrency, observability, and maintainable architecture.
</p>

<p align="center">
  <a href="https://linkedin.com/in/tahagurvardar">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="https://github.com/tahagurvardar/forgegrid">
    <img src="https://img.shields.io/badge/ForgeGrid-v1.0.0-2EA043?style=for-the-badge&logo=github&logoColor=white" alt="ForgeGrid" />
  </a>
  <a href="https://github.com/tahagurvardar/racelab">
    <img src="https://img.shields.io/badge/RaceLab-v2.0.0-2EA043?style=for-the-badge&logo=github&logoColor=white" alt="RaceLab" />
  </a>
</p>

---

## 👨‍💻 About Me

- 🎓 Computer Engineering student at **Khazar University**
- ⚙️ Building distributed systems, backend infrastructure, real-time desktop software, and full-stack applications
- 💻 Working with **Go, Rust, TypeScript, React, PostgreSQL, gRPC, Docker, and Tauri**
- 🌐 Interested in **distributed systems, concurrency, networking, backend architecture, observability, and developer tooling**
- 🔐 Focused on correctness, failure handling, secure boundaries, and maintainable software
- 🌍 Open to internships, junior software engineering roles, backend/systems opportunities, and remote work

---

## 🛠️ Technology Stack

### Systems & Backend

<p>
  <img src="https://skillicons.dev/icons?i=go,rust,nodejs,postgres,docker,redis&perline=6" alt="Systems and backend stack" />
</p>

`Go` · `Rust` · `Node.js` · `PostgreSQL` · `gRPC` · `Docker` · `Redis`

### Frontend

<p>
  <img src="https://skillicons.dev/icons?i=nextjs,react,ts,js,tailwind,html,css,vite&perline=8" alt="Frontend stack" />
</p>

`Next.js` · `React` · `TypeScript` · `JavaScript` · `Tailwind CSS` · `HTML` · `CSS` · `Vite`

### Data & Persistence

<p>
  <img src="https://skillicons.dev/icons?i=postgres,prisma,mongodb,sqlite,redis&perline=5" alt="Data stack" />
</p>

`PostgreSQL` · `Prisma` · `MongoDB` · `SQLite` · `Redis` · `IndexedDB`

### Desktop, Networking & Infrastructure

<p>
  <img src="https://skillicons.dev/icons?i=rust,tauri,docker&perline=3" alt="Desktop and infrastructure stack" />
</p>

`Rust` · `Tauri` · `Docker` · `gRPC` · `UDP` · `SSE` · `Web Workers` · `Windows`

### Observability, Testing & Delivery

<p>
  <img src="https://skillicons.dev/icons?i=prometheus,grafana,vitest,githubactions,git,github,vercel&perline=7" alt="Observability, testing and delivery stack" />
</p>

`OpenTelemetry` · `Prometheus` · `Jaeger` · `Playwright` · `Vitest` · `GitHub Actions` · `Git`

### Languages

<p>
  <img src="https://skillicons.dev/icons?i=go,ts,js,rust,python,java,cs,c&perline=8" alt="Programming languages" />
</p>

`Go` · `TypeScript` · `JavaScript` · `Rust` · `Python` · `Java` · `C#` · `C`

---

## 🚀 Featured Projects

### ⚙️ ForgeGrid — Distributed Job Execution Engine

A distributed job execution platform focused on **execution ownership, worker failure recovery, concurrency, and observability**.

- Go Control Plane and Worker agents communicating over **gRPC**
- PostgreSQL-backed durable coordination and scheduling
- Heartbeat-based worker liveness detection
- Renewable execution leases and monotonic fencing tokens
- Worker session/incarnation tracking
- Bounded infrastructure retries and stale-result rejection
- Static DAG pipelines with fan-out, fan-in, dependency release, cancellation, and timeout semantics
- Docker-based isolated execution for trusted workloads
- Live stdout/stderr streaming over bounded SSE
- Worker crash recovery with reassignment to another worker
- Distributed tracing with **OpenTelemetry**
- Metrics with **Prometheus**
- Trace inspection with **Jaeger**
- React operational console for pipelines, workers, attempts, logs, and recovery history
- Real recovery verification:
  `worker-b / LOST / fence 1 → worker-c / SUCCEEDED / fence 2`

ForgeGrid provides **at-least-once physical execution with a single authoritative attempt**. It intentionally does not claim exactly-once execution, hostile multi-tenant isolation, or production HA.

<p>
  <a href="https://github.com/tahagurvardar/forgegrid">
    <img src="https://img.shields.io/badge/Repository-ForgeGrid-181717?style=for-the-badge&logo=github&logoColor=white" alt="ForgeGrid repository" />
  </a>
  <a href="https://github.com/tahagurvardar/forgegrid/releases/tag/v1.0.0">
    <img src="https://img.shields.io/badge/Release-v1.0.0-2EA043?style=for-the-badge&logo=github&logoColor=white" alt="ForgeGrid v1.0.0" />
  </a>
</p>

---

### 🏎️ RaceLab — Real-Time Motorsport Telemetry for Windows

A Windows telemetry, automatic session recording, and in-game overlay application for **F1 25** and **Forza Horizon 6**.

- Real-time UDP telemetry ingestion
- Automatic game and session detection
- Automatic session recording and persistence
- Mixed-game session history
- F1 lap, sector, event, tyre, fuel, ERS, and vehicle-state data
- Click-through in-game F1 overlay
- Bounded background telemetry and recording workers
- Local-first storage and retention
- Built with **Rust, Tauri, React, and TypeScript**

<p>
  <a href="https://github.com/tahagurvardar/racelab">
    <img src="https://img.shields.io/badge/Repository-RaceLab-181717?style=for-the-badge&logo=github&logoColor=white" alt="RaceLab repository" />
  </a>
  <a href="https://github.com/tahagurvardar/racelab/releases/tag/v2.0.0">
    <img src="https://img.shields.io/badge/Release-v2.0.0-2EA043?style=for-the-badge&logo=github&logoColor=white" alt="RaceLab v2.0.0" />
  </a>
</p>

---

### 🎟️ SeatFlow — Transactional Event Ticketing Platform

A multi-tenant event ticketing platform centered on **atomic inventory, transactional consistency, and auditable financial workflows**.

- Versioned venues and immutable seat maps
- PostgreSQL-backed atomic seat holds
- Concurrent inventory protection with row locking
- Simulated payment provider and verified webhook processing
- Exact-once booking fulfillment at the application boundary
- QR tickets and atomic first-use redemption
- Refunds, disputes, financial ledger, and reconciliation
- Background jobs and transactional outbox workflows
- Tenant-scoped authorization

<p>
  <a href="https://github.com/tahagurvardar/seatflow">
    <img src="https://img.shields.io/badge/Repository-SeatFlow-181717?style=for-the-badge&logo=github&logoColor=white" alt="SeatFlow repository" />
  </a>
  <a href="https://seatflow-staging.vercel.app">
    <img src="https://img.shields.io/badge/Live%20Demo-SeatFlow-2EA043?style=for-the-badge&logo=vercel&logoColor=white" alt="SeatFlow demo" />
  </a>
</p>

---

### 🧭 CommitTrail — Evidence-Backed Engineering Portfolio

A full-stack platform for turning repository activity into structured, inspectable, evidence-backed engineering stories.

- GitHub App integration
- Durable PostgreSQL background worker
- HMAC-verified webhooks
- Bounded retries and idempotent reconciliation
- Evidence provenance
- Versioned public profiles and projects
- Workspace-scoped authorization
- Privacy-aware publishing
- Deterministic CV and interview outputs
- Built with **Next.js, PostgreSQL, Prisma, and Better Auth**

<p>
  <a href="https://github.com/tahagurvardar/committrail">
    <img src="https://img.shields.io/badge/Repository-CommitTrail-181717?style=for-the-badge&logo=github&logoColor=white" alt="CommitTrail repository" />
  </a>
  <a href="https://committrail.vercel.app">
    <img src="https://img.shields.io/badge/Public%20Demo-CommitTrail-2EA043?style=for-the-badge&logo=vercel&logoColor=white" alt="CommitTrail demo" />
  </a>
</p>

---

### ⚙️ QueueForge — Deterministic Operations Simulation

A browser-based discrete-event simulation for comparing scheduling strategies under reproducible workloads.

- Pure deterministic simulation engine
- Seeded workload generation
- Stable event scheduling
- FIFO and SEPT-with-ageing strategies
- Dedicated Web Worker execution
- Same-workload strategy comparison
- Deterministic replay verification
- Browser-local IndexedDB persistence
- Versioned JSON and CSV exports

<p>
  <a href="https://github.com/tahagurvardar/queueforge">
    <img src="https://img.shields.io/badge/Repository-QueueForge-181717?style=for-the-badge&logo=github&logoColor=white" alt="QueueForge repository" />
  </a>
  <a href="https://queueforge-five.vercel.app">
    <img src="https://img.shields.io/badge/Live%20Demo-QueueForge-2EA043?style=for-the-badge&logo=vercel&logoColor=white" alt="QueueForge demo" />
  </a>
</p>

---

### 🧩 WordX — Bilingual Word Puzzle

An original Turkish and English word puzzle with multiple game modes.

- Classic
- Quick Rush
- Daily Challenge
- Guest gameplay
- Optional account system
- Game history and achievements

<p>
  <a href="https://github.com/tahagurvardar/wordx">
    <img src="https://img.shields.io/badge/Repository-WordX-181717?style=for-the-badge&logo=github&logoColor=white" alt="WordX repository" />
  </a>
  <a href="https://wordx-staging.vercel.app">
    <img src="https://img.shields.io/badge/Staging-WordX-2EA043?style=for-the-badge&logo=vercel&logoColor=white" alt="WordX staging" />
  </a>
</p>

---

## 📂 Other Projects

- [CareerBridge](https://github.com/tahagurvardar/careerbridge) — hiring platform with role-based workflows
- [Smart Product Intelligence](https://github.com/tahagurvardar/smart-product-intelligence) — applied machine learning project
- [WorldCupManager 2026](https://github.com/tahagurvardar/WorldCupManager-2026) — national-team management platform
- [TurcoManager](https://github.com/tahagurvardar/TurcoManager) — football-management simulation
- [Virtual Memory Manager](https://github.com/tahagurvardar/Virtual-Memory-Manager) — virtual-memory simulation

---

## 🎯 Engineering Focus

- Distributed systems and fault tolerance
- Backend infrastructure
- Concurrency and transactional correctness
- Real-time networking and telemetry
- PostgreSQL coordination and persistence
- Worker scheduling and background processing
- Observability and distributed tracing
- Deterministic simulation
- Desktop and native software
- Full-stack product engineering
- Automated testing and adversarial failure testing

---

## 🔬 What I Like Building

Systems where correctness matters when things go wrong:

- workers disappearing during execution
- concurrent requests racing for the same resource
- network connections dropping
- retries delivering duplicate messages
- stale processes returning late results
- real-time data arriving continuously
- state needing to survive process failures

I enjoy designing the ownership rules, persistence boundaries, failure behavior, and tests that make these systems understandable and reliable.

---

## 🎓 Education

**Computer Engineering — Khazar University, Baku**

Relevant coursework includes Software Engineering, Data Structures and Algorithms, Database Systems, Operating Systems, Computer Networks, Computer Organization, Artificial Intelligence, Neural Networks, Distributed Systems, and Information Security.

---

## 📫 Contact

<p>
  <a href="https://linkedin.com/in/tahagurvardar">
    <img src="https://img.shields.io/badge/LinkedIn-Taha%20Gürvardar-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
</p>
