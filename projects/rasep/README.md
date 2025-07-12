# Rasep – Supply Chain Automation System 🚚📦

Rasep is a logistics backend platform designed to manage warehouse operations, track orders, and coordinate drivers for real-time delivery updates. Built using modern, scalable technologies with a Hasura-ready architecture.

## ⚙️ Tech Stack

- **Backend**: Node.js, NestJS
- **Database**: PostgreSQL
- **Frontend**: React (admin panel & tracking UI)
- **Real-time**: Webhooks, Hasura Events (PoC)
- **Monitoring**: Custom health endpoints + logs

## 🔑 Key Features

- Real-time order lifecycle management (Create → Dispatch → Deliver)
- Warehouse inventory tracking with SKU-level details
- Driver assignment and live route updates
- Admin dashboard for order, location, and status visualization
- PoC integration with Hasura for auto-generated GraphQL APIs
- Webhook support for delivery notifications and partner sync

## 🧠 System Highlights

- NestJS modules for Orders, Drivers, Inventory, and Notifications
- PostgreSQL schema with relational integrity and transaction safety
- Hasura integration with auth headers, event triggers, and custom resolvers
- Graceful fallback on webhook retries with exponential backoff
- Status tracking: `OrderStatus = [Placed → Packed → Dispatched → Delivered]`

## 👨‍💻 My Role

- Architected the backend with modular NestJS services
- Implemented inventory ledger and real-time dispatch flows
- Integrated Hasura PoC for GraphQL clients
- Designed PostgreSQL schema for orders, products, and driver routes
- Wrote robust error handlers and monitoring endpoints

## 📦 Deployment

```bash
docker-compose up
