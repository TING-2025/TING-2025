# FingerprintVS Project

Welcome to the **FingerprintVS Virtual System**!  
A hybrid biometric fingerprint capture, verification, and authentication system designed for secure fingerprint scanning across both web and local installations.

---

## 🔥 About Me
-👋 Hi, I’m @TING-2025
- **Name**: Leilan Robinson
- **Company**: Trusted Independent Networking Group
- **Role**: Founder, Lead Developer, System Architect & Cybersecurity Analyst
- **Background**: 7+ years in cybersecurity, biometrics, network architecture, and Python development.  
  Certified Ethical Hacker (CEH) | Certified Cloud Security Professional (CCSP)
- **Interests**: Biometrics, Cybersecurity, Cloud Infrastructure, Python Development, DevOps Automation

---

## 📚 Project Overview

FingerprintVS Virtual System is designed to:

- 🖐️ Capture fingerprint data using Suprema RealScan G10 devices
- 🛠️ Process, enhance, and validate fingerprint images against quality standards
- 🗄️ Securely store fingerprint templates (SQLite/MySQL with encryption)
- 🔍 Match fingerprints and authenticate users with high accuracy
- 🌐 Integrate with WordPress + Vue.js frontend for user management and reporting
- 📢 Send alerts (Email/SMS/Push) on capture issues or authentication anomalies

---

## 🛠️ Tech Stack

- **Programming Language**: Python 3.11
- **Backend**: Flask (API layer) + FastAPI (optional async features)
- **Database**: SQLite (prototype), MySQL 8.0+ (production)
- **Frontend**: WordPress + Vue.js (user dashboard, subscription, notifications)
- **Biometric SDK**: Suprema G-SDK v1.7.1 (Python Client)
- **Cloud Hosting**: Oracle Cloud (Ubuntu 24.04 LTS VM)
- **Security**: SSL Certificates (Let's Encrypt/Custom CA), Token Auth, Optional WAF

---

## 📋 Project Structure

```bash
FingerprintVS/
├── device_gateway/
│   ├── device_gateway_x64.exe
│   └── biostar/
│       ├── gateway_pb2_grpc.py
│       ├── gateway_pb2.py
│       └── __init__.py
├── cert/
│   ├── ca.crt
│   ├── ca_key.pem
│   ├── server.crt
│   ├── server_key.pem
│   └── eula.accepted
├── app/
│   ├── app.py (Flask API server)
│   ├── models.py
│   ├── routes.py
│   └── utils.py
├── fingerprints.db (SQLite database)
├── .env (Environment Variables)
├── requirements.txt
└── README.md (this file)
```

---

## 🛡️ Features

- **Portable Flash Drive Version**: Fully offline, encrypted
- **Web-Based Version**: Hosted, auto-updating with SSL
- **Installed System**: Office LAN, offline secure operation
- **Real-Time Alerts**: Email, SMS, Push notifications
- **NIST Fingerprint Quality Validation**: ISO/IEC 19794-2, FBI IAFIS standards
- **Secure Encrypted Storage**: AES-256 encryption for templates and logs

---

## 🚀 Deployment Options

- **Flash Drive**: Bootable, encrypted offline version
- **Web-Based Cloud**: SSL-secured hosted API + WordPress frontend
- **Office LAN**: Local Gateway server for intranet access

---

## 📈 Current Milestones

- [x] Oracle VM setup and server hardening
- [x] Suprema Device SDK operational
- [x] Initial Flask API live
- [x] Python Client / gRPC Gateway communication
- [ ] Integrate gRPC server with Port 4000/51212
- [ ] Flask endpoint testing (capture, match)
- [ ] WordPress API user syncing
- [ ] Alerts & Reporting API (SMTP/Twilio)
- [ ] Final QA + Production Deployment

---

## 📌 Important Developer Notes

- ✅ Full name and background info added
- ⚡ Ensure `config.json` matches Port 4000 (gRPC) and SSLPort 51213
- ⚡ Certificates (.crt/.pem) must be correctly located in `/cert/`
- ⚡ Environment variables (.env) must store sensitive data (DB, API keys)
- ⚡ Firewall/UFW must allow inbound Port 4000 and 51212
- ⚡ Set device reconnect interval >30 seconds (config file)
- ⚡ Ensure alert systems (SMTP, Twilio) have API keys + IP whitelist
- ⚡ Schedule backups for `fingerprints.db`
- ⚡ Add SDKs (JS/Python) for future frontend integrations

---

## 📞 Contact

- **Email**: info@fingerprintVS.com
- **Web**: [https://fingerprintvs.com](https://fingerprintvs.com)
- **GitHub**: Trusted Independent Networking Group GitHub

---

# 🚀 Let's make FingerprintVS a secure, powerful, industry-leading biometric solution!

<!---
TING-2025/TING-2025 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
