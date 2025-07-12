# Blush Now – Beauty Booking & Loyalty Platform 💄📅

Blush Now is a full-featured backend system for a beauty and salon service platform, enabling users to schedule appointments, make payments, and earn loyalty rewards.

## ⚙️ Tech Stack

- **Backend**: Node.js, Express.js
- **Payments**: Stripe (Subscriptions & One-time payments)
- **Database**: Redis (sessions, rate-limiting), PostgreSQL
- **Admin Interface**: Forest Admin
- **Monitoring**: Sentry, Winston Logging

## 🔑 Key Features

- Booking APIs with slot locking, availability lookup, and calendar sync
- Loyalty engine (referral + credit-based reward system)
- Promo code and seasonal discount engine
- Stripe payment integration with retry and webhook flow
- Admin panel setup via Forest Admin for service staff and order tracking
- Sentry-based real-time error logging and alerting

## 🧠 System Highlights

- Redis used for locking time slots and preventing overbooking
- Stripe checkout and webhook-based subscription verification
- Modular services for appointment, invoice, payment, and reward systems
- Sentry used for stack trace capture and Slack alert integration
- JWT-based authentication and scoped roles (admin vs customer)

## 👨‍💻 My Role

- Built backend APIs for appointment lifecycle and loyalty tracking
- Integrated Stripe billing and webhook-based payment verification
- Created dynamic discount rules and reward tracking logic
- Configured Forest Admin with access control for operations team
- Implemented structured logging and Sentry error monitoring

## 📦 Deployment

```bash
docker-compose up
