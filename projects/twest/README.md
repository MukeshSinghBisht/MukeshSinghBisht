# Twest – Crypto Finance Platform 💰📉

Twest is a real-time cryptocurrency finance platform enabling users to manage assets, complete KYC, and perform secure fiat/crypto transactions. Designed for performance, scalability, and security with Dockerized microservices.

## ⚙️ Tech Stack

- **Backend**: Node.js, Express.js
- **Database**: MySQL
- **Containerization**: Docker, Docker Compose
- **Security**: JWT Auth, Secure APIs
- **DevOps**: Shell scripts, Nginx (reverse proxy), Docker volumes

## 🔑 Key Features

- User authentication and KYC flow with secure onboarding
- Portfolio tracker for live crypto and fiat balances
- Transaction engine supporting deposits, withdrawals, and transfers
- Rate fetching from external APIs (CoinGecko, Binance, etc.)
- Background jobs for transaction reconciliation and email alerts
- Admin dashboard for monitoring balances and activities (basic)

## 🧠 System Highlights

- Modular route/controllers/services separation in Express.js
- Token-based authentication with middleware for RBAC
- MySQL schema for users, balances, transactions, KYC status
- Docker setup for consistent local and production deployment
- Shell utilities for backup, restore, and DB migration

## 👨‍💻 My Role

- Designed and implemented secure REST APIs for finance modules
- Integrated crypto price API and balance tracker
- Set up Docker-based environment with volume persistence
- Handled transaction consistency and rollback mechanisms
- Led API documentation and collaboration with frontend team

## 🚀 Local Setup

```bash
git clone https://github.com/MukeshSinghBisht/twest-crypto-finance.git
cd twest-crypto-finance
docker-compose up --build
