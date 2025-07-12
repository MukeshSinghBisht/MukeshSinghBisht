# Call48 – Telecom SaaS for PBX & DID Management 📞🔧

Call48 is a backend telecom system enabling DID (Direct Inward Dialing) management and PBX automation for VoIP service providers and call centers.

## ⚙️ Tech Stack

- **Backend**: Node.js, Express.js, Sequelize
- **Database**: PostgreSQL, Redis
- **Infrastructure**: Docker, PM2, Nginx
- **Other**: REST APIs, JWT, Webhooks, Load Balancing

## 🔑 Key Features

- DID pool management and intelligent number allocation
- Concurrent DID purchase flow with auto-retry and validation
- Real-time call routing configuration APIs
- Load-aware DID availability lookup using Redis caching
- Secure webhook integration with telecom providers
- Admin dashboard-ready API layer (multi-tenant support)

## 🧠 System Highlights

- Redis used for tracking high-concurrency purchase flow with TTL-based locks
- Sequelize-based dynamic query builder for flexible filtering
- Modular service structure for billing, call routing, and DID validation
- Graceful failure handling and email alerts for blocked DIDs
- Docker-based staging and production environments

## 👨‍💻 My Role

- Designed and implemented 10+ APIs for DID allocation, routing, and billing
- Developed Redis lock logic to prevent race conditions during high traffic
- Refactored core modules to support multi-tenant logic
- Mentored junior devs and documented onboarding modules
- Interfaced with external SIP/DID providers via secure webhook systems

## 📦 Deployment

```bash
docker-compose up -d
