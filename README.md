# ☁️ Cloud Resume Challenge (Azure Edition)

This project is my completed version of the **Cloud Resume Challenge**, a hands-on, end-to-end cloud engineering exercise that tests your skills across front-end, back-end, CI/CD, Infrastructure as Code, and cloud architecture. I used **Microsoft Azure** for cloud services and **GitHub Actions** for automation, and wrapped everything with a secure and custom domain via **Cloudflare**.

📎 Live Project: [resume.zakjaeb.com](https://resume.zakjaeb.com)

---

## 🔧 Tech Stack

- **Frontend**: HTML/CSS static resume site (Azure Static Web App)
- **Backend**: Azure Functions (Python) + Cosmos DB (Table API)
- **CI/CD**: GitHub Actions
- **Infra as Code**: ARM templates
- **Testing**: Cypress smoke tests
- **Security**: DNSSEC, HTTPS enforced via Cloudflare

---

## 📌 Challenge Summary

Over five days, I built and deployed a full-stack cloud project from scratch:

1. **Day 1 – Static Site + Domain Setup**
   - Deployed resume to Azure Storage as a static website
   - Configured custom domain (`resume.zakjaeb.com`) with Cloudflare
   - Troubleshot CNAME verification and DNS resolution
   - Enabled HTTPS and DNSSEC for added security

2. **Day 2 – Visitor Tracking API**
   - Created Azure Functions to track and return visitor count
   - Connected Function App to Cosmos DB (Table API)
   - Fixed connection string issues and enabled CORS
   - Integrated API with frontend using JavaScript

3. **Days 3–5 – CI/CD, IaC, and Testing**
   - Restructured into mono-repo: `frontend/`, `backend/`, `infra/`, `cypress/`
   - Wrote ARM templates to deploy Function App and Cosmos DB
   - Created GitHub Actions workflows:
     - Deploy infrastructure (ARM)
     - Deploy Azure Function App
     - Deploy static site
     - Run Cypress smoke tests (manual for now)
   - Secured workflows with GitHub Secrets + Azure Service Principal

---

## 🧠 Key Lessons

- Visualizing and debugging DNS across Cloudflare + Azure is tricky — but essential.
- Azure Function Apps + Cosmos DB are powerful (once the connection string is right).
- CI/CD with GitHub Actions is worth the setup — infrastructure becomes repeatable.
- A mono-repo structure simplifies maintenance and scaling.

---

## 🚀 Repo Structure

```
cloud-resume-challenge/
│
├── frontend/            # Static HTML/CSS resume site
├── backend/             # Azure Functions (Python)
├── infra/               # ARM templates for deployment
├── cypress/             # Cypress smoke tests
└── .github/workflows/   # GitHub Actions workflows
```

---

## 📸 Screenshots

*Coming soon — CI/CD pipeline diagrams and DNS flow visuals.*

---

## 🔐 Note

This repo is currently private due to Cosmos DB credentials. A sanitized public version with dummy config values and full documentation is in the works!

---

## 🙏 Thanks

Big thanks to [Forrest Brazeal](https://forrestbrazeal.com) for designing the challenge and to the cloud community for sharing their builds and insights.

---

## 📣 Want to Connect?

If you're building this or something similar, reach out!  
👉 [zakjaeb.com](https://zakjaeb.com) | [LinkedIn](https://linkedin.com/in/zakjaeb) | [YouTube](https://youtube.com/@zakjaeb)
