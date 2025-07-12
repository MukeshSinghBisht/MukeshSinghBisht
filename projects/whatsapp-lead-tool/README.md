# WhatsApp Lead Tool 📲

A lightweight, scalable lead generation and management system built around WhatsApp links. The platform enables users to create personalized WhatsApp URLs, track incoming leads, manage statuses, and export data.

## 🚀 Tech Stack

- **Backend**: Node.js, GraphQL, Hasura, Kafka, MongoDB, Redis
- **Frontend**: Next.js, Redux, TailwindCSS
- **Infra**: Docker, Kafka, Hasura Event Triggers, Webhooks

## 🔧 Key Features

- WhatsApp link generator with customizable prefilled messages
- Lead capture from incoming messages or form entries
- Lead status management with tagging and filtering
- CSV export of captured leads
- Kafka-based retry & DLQ mechanism for fault tolerance
- Analytics: count by status, tags, and lead sources
- Basic authentication (magic link or Google Sign-In)
- Scalable architecture using Hasura & microservices

## 🧩 Architecture Overview

- Event-driven backend using Kafka
- Hasura auto-generates GraphQL APIs from PostgreSQL
- DLQ (dead letter queue) for failed message capture
- Admin dashboard to manage leads and view analytics
- Redux-Saga for managing side effects and API communication

## 🔍 Highlights

- Built for multi-user use with role-based permissions
- Modular folder structure to scale new lead channels (email, SMS)
- Integrates with WhatsApp Web via deep linking
- Future-proof: easily extendable with GPT/NLP-based lead enrichment

## 👨‍💻 My Role

- Designed system architecture from scratch
- Implemented core Kafka consumers and Hasura event triggers
- Developed GraphQL APIs, lead retry flows, and tagging filters
- Built the lead dashboard and export logic

## 📦 Deployment

Can be deployed using Docker Compose locally or on any cloud platform.
