# Hi there, I'm Carlos Murillo 👋

<p align="left">
  <strong>Senior Full-Stack, Mobile & Systems Engineer</strong><br>
  <em>Specializing in High-Performance TypeScript/React, Native Android / React Native & Smart Contracts (Rust, Solana, Soroban)</em>
</p>

<p align="left">
  <a href="https://www.upwork.com/freelancers/~0170d6b02e9440e604">
    <img src="https://img.shields.io/badge/Upwork-Verified%20Freelancer-14a800?style=flat-square&logo=upwork&logoColor=white" alt="Upwork Profile" />
  </a>
  <img src="https://img.shields.io/badge/GitHub-Member%20Since%202011-2ea44f?style=flat-square&logo=github&logoColor=white" alt="Member Since 2011" />
  <img src="https://img.shields.io/badge/Open%20Source-30%2B%20Merged%20PRs-blue?style=flat-square&logo=git&logoColor=white" alt="Merged PRs" />
  <a href="https://solagent-sentinel.vercel.app">
    <img src="https://img.shields.io/badge/Live%20Demo-SolAgent%20Sentinel-blueviolet?style=flat-square&logo=vercel&logoColor=white" alt="Live Demo" />
  </a>
</p>

---

### 👨‍💻 About Me

I am a senior software and systems engineer with over a decade of industry experience (GitHub member since 2011). My background spans enterprise private architecture, native mobile application engineering, and open-source systems programming.

Today, my core focus is delivering robust production software across three primary domains:
* 📱 **Mobile & Cross-Platform Engineering**: Native Android development (Kotlin, Jetpack Compose, Android Auto / `CarAppService`) and cross-platform apps with **React Native** & TypeScript.
* ⚡ **Full-Stack & Distributed Systems**: Scalable web applications using **React**, **Next.js**, **Node.js**, and relational databases (**PostgreSQL**, Row Level Security, transactional advisory locks).
* 🦀 **Web3 & Systems Security**: Secure smart contract protocols in **Rust** on **Solana** (Anchor framework, PDA security, AST instruction heuristics) and **Stellar Soroban** (state persistence, TTL rent management, escrow logic).

---

### 🛠️ Technical Stack & Tooling

```text
Languages:          TypeScript, JavaScript, Rust, Kotlin, SQL
Mobile & Frontend:  React Native, Android (Jetpack Compose, Android Auto), React, Next.js, Tailwind CSS
Backend & Cloud:    Node.js, Express, PostgreSQL (Advisory Locks, RLS), Supabase, Redis, REST APIs
Web3 & Protocols:   Solana (Anchor, Web3.js), Stellar (Soroban SDK, Horizon/RPC)
Testing & CI/CD:    Jest, Vitest, Cargo Test, GitHub Actions, Docker, ESLint
```

---

### 🌟 Featured Original Projects

#### 🛡️ [SolAgent Sentinel](https://github.com/camesenin/solagent-sentinel)
> **Autonomous pre-flight security agent & AST firewall for Solana Actions (Blinks) and autonomous AI trading agents.**  
> * **Tech**: Rust, Solana Anchor, TypeScript, Next.js 14, Tailwind CSS, Vercel.  
> * **Architecture**: Deconstructs transaction Abstract Syntax Trees (AST) in memory to intercept malicious `SetAuthority` wallet drainers and unlimited allowances before signing.
> * **Performance**: Benchmarked at **0.028 – 0.038 ms** in-memory AST evaluation latency with zero false positives. Detailed methodology, hardware specifications, and reproducible test commands are documented in [BENCHMARK.md](https://github.com/camesenin/solagent-sentinel/blob/main/BENCHMARK.md).
> * **Artifacts**: Anchor Devnet registry contract, dual-perspective inspector (End-User mode vs. Security Auditor mode), and automated test suite.  
> * 🔗 **Live App**: [solagent-sentinel.vercel.app](https://solagent-sentinel.vercel.app) · **Repo**: [camesenin/solagent-sentinel](https://github.com/camesenin/solagent-sentinel)

#### 🏍️ [MotoECU](https://github.com/camesenin/MotoECU)
> **Native Android telemetry, diagnostic & trip analytics engine with Android Auto projection support.**  
> * **Tech**: Kotlin, Jetpack Compose, Android Auto (`CarAppService`), Bluetooth Classic / BLE, Room SQLite, Coroutines.  
> * **Architecture**: Interfaces with motorcycle ECU via Bluetooth ELM327 OBD-II protocols. Implements real-time telemetry streaming, exponential moving average (EMA) filters for noise reduction, and background foreground services with SQLite persistence for trip logs.
> * **Features**: Custom heads-up automotive dashboard, DTC trouble code reader/clearer, and CSV export for telemetry analysis.  
> * 🔗 **Repo**: [camesenin/MotoECU](https://github.com/camesenin/MotoECU)

---

### 🔬 Technical Case Studies: Merged Open-Source Contributions

Rather than superficial commits, my open-source work focuses on solving complex architecture, concurrency, and security challenges:

#### 1. Concurrency Control & Database Migration Integrity — [StellarCore](https://github.com/camesenin/StellarCore)
* **Challenge**: Multi-threaded anchor processors running concurrent synchronization jobs suffered potential race conditions during ledger ingestion and schema migrations.
* **Architectural Decision**: Implemented PostgreSQL namespaced transaction advisory locks (`pg_try_advisory_xact_lock`) ensuring strict transactional idempotency across parallel worker threads without causing table lock escalation. Added automated pre-migration validation checks.
* **Impact**: Zero deadlocks under concurrent simulation, deterministic migration rollbacks.

#### 2. Cloud Security & On-Chain State Rent Defense — [Orbit Protocol](https://github.com/Orbit-xyz/Orbit)
* **Challenge**: Decentralized pull payment vaults on Stellar Soroban faced state eviction risks under ledger TTL expirations, alongside multi-tenant security vulnerabilities in API endpoints.
* **Architectural Decision**: Engineered automated contract state TTL rent extension handlers executed during `batch_disburse` workflows. Hardened the Supabase PostgreSQL backend by establishing least-privilege Row Level Security (RLS) policies. Eliminated zero-share division arithmetic edge cases.
* **Impact**: Guaranteed state persistence for recurring payout schedules and locked down customer vault records.

#### 3. High-Throughput Stream Exports & Community Governance — [Stolla](https://github.com/stolla-labs/stolla)
* **Challenge**: Large community proposal datasets produced client memory spikes and lacked export capabilities for DAO audit compliance.
* **Architectural Decision**: Engineered client-side streaming CSV and JSON export pipelines with sanitized character parsing and chunked payload processing. Integrated vote delegation permission checks with optimistic UI updates.
* **Impact**: Eliminated browser rendering lag for communities with 1,000+ proposals and enabled one-click compliance exports.

---

### 🏢 Ongoing Enterprise Collaboration

* **[Expensify / App](https://github.com/Expensify/App)**: Active contributor to the next-generation financial collaboration platform built on **React Native**, **TypeScript**, and **Onyx** state management. Focusing on root-cause analysis, cross-platform UI synchronization (Web, Android, iOS), and reproducible issue remediation.

---

### 📬 Connect With Me

* 💼 **Upwork**: [Carlos M. Profile](https://www.upwork.com/freelancers/~0170d6b02e9440e604)
* 🐙 **GitHub**: [@camesenin](https://github.com/camesenin)
* 🌐 **Live Demo**: [SolAgent Sentinel](https://solagent-sentinel.vercel.app)
