# AI-Powered IDS

### 📌 About
AI-Powered IDS (Intrusion Detection System) is a backend-integrated, machine learning-based system designed to detect and flag suspicious activity from incoming requests. Built to plug into modern Node.js APIs, it helps identify anomalies like brute-force attacks, request floods, or abnormal access patterns.

---

### ✨ Features
- Real-time log analysis for suspicious API calls
- Machine learning-based anomaly detection (Isolation Forest)
- Middleware-ready for Express/NestJS backends
- Alerts based on IP, frequency, and payload patterns
- CLI support for model training and log simulation

---

### 🛠 Stack
- **Backend:** Node.js (Express/NestJS)
- **AI/ML:** Python (scikit-learn, pandas)
- **Storage:** MongoDB / CSV
- **Tooling:** Redis/Kafka (optional), Winston logger
- **Scripts:** Python scripts for model training & log simulation

---

### 🔧 Responsibilities
- Designed a modular IDS middleware to plug into any Node.js or NestJS app
- Trained and saved ML model using Isolation Forest to detect behavioral anomalies
- Built request logger to capture, store, and feed structured logs to ML model
- Configured automatic IP banning or webhook alerts for repeated suspicious activity
- Simulated real-world attack traffic to evaluate and improve model precision

---

### 📈 Outcome
- Enabled real-time security monitoring of API endpoints
- Reduced manual log auditing effort by 70%
- Laid the foundation for integrating with ELK or Prometheus-Grafana stack
- Helped backend systems proactively block or alert on attack vectors

---

### 🔗 Related
- [Train model script](./model/train_model.py)
- [Node.js Middleware](./src/idsMiddleware.js)
- [Log simulation tool](./scripts/simulate_traffic.py)

---

> This project demonstrates how to apply machine learning to production-level Node.js backends for proactive threat detection.
