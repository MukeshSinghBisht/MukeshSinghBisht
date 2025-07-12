# Secpay – Crypto Payment Plugin System 💳🔐

A secure, modular crypto payment system for WooCommerce and Shopify. Built with compliance in mind, it integrates TRISA protocols and uses AWS-native serverless infrastructure.

## 🚀 Tech Stack

- **Backend**: Node.js, TypeScript, gRPC, Serverless Framework
- **Cloud**: AWS Lambda, Step Functions, EC2, DynamoDB, S3
- **Compliance**: TRISA Protocol, TDD
- **Other**: GitHub Actions (CI/CD), JWT Auth, Webhooks

## 🔧 Key Features

- Crypto-to-fiat plugins for Shopify and WooCommerce
- TRISA-compliant identity validation and transaction recording
- Step Functions-based transaction state machine (initiate, validate, complete, fail)
- Retry mechanism for failed transactions using serverless retries
- Secure encrypted API key handling and webhook callbacks
- Audit logs and alert notifications
- Full plugin API with merchant-specific endpoints
- Test-driven with 90%+ code coverage

## 🧩 Architecture Overview

- **Lambda functions** handle payment initiation, transaction validation, and wallet callbacks
- **Step Functions** manage the entire transaction flow using state transitions
- **DynamoDB** stores transaction records with TTL and status fields
- **gRPC** used for internal secure plugin communications
- CI/CD via GitHub Actions with automatic rollback on failure

## 👨‍💻 My Role

- Designed the entire plugin transaction state machine
- Implemented gRPC interface and Lambda handlers with TypeScript
- Developed retry logic using Step Function error states
- Integrated TRISA ID verification and test coverage suite
- Maintained secure deployment via Serverless Framework and AWS Secrets Manager

## 📦 Deployment

Serverless deploy on AWS using:

```bash
npm install
serverless deploy --stage prod
