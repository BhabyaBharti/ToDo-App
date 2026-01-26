# Production-Grade DevSecOps CI/CD Pipeline  
### Full-Stack Application Delivery with Azure DevOps & GitHub Actions

---

## 🚀 Why This Repository Exists

In real enterprise environments, **applications are easy — delivery is hard**.

This repository is intentionally built to **demonstrate how production-grade CI/CD pipelines are designed**, secured, and operated for real-world applications.

> 🔴 The application is deliberately simple.  
> 🟢 The pipeline is intentionally complex.

The primary focus here is **DevSecOps, quality gates, artifact governance, approval workflows, and VM-based deployments**, not application features.

---

## 🧠 Problem Statement (Real-World Context)

Modern delivery teams face challenges such as:
- Preventing vulnerable dependencies from reaching production
- Enforcing consistent quality standards across stacks
- Managing approvals and auditability
- Ensuring reliable deployments to long-lived environments (VMs)
- Balancing speed with security

This repository simulates those challenges and demonstrates **how CI/CD pipelines solve them**.

---

## 🏗️ Application Overview (Delivery Vehicle)

The application serves only as a **delivery vehicle** for the pipeline.

- **Frontend:** React  
- **Backend:** Python (FastAPI / Uvicorn style)  
- **Containerization:** Docker  
- **Deployment Target:** Azure Virtual Machines  
- **Extensible To:** AWS EC2, Containers, Kubernetes  

---

## 🔄 What This Repository Demonstrates (DevOps Scope)

This project showcases **enterprise-grade CI/CD capabilities**, including:

✅ Stage-based pipeline architecture  
✅ Software Composition Analysis (Retire.js)  
✅ Static Code Analysis (SonarQube / SonarCloud)  
✅ Extensive linting & quality checks  
&nbsp;&nbsp;&nbsp;&nbsp;• ESLint, Stylelint, Biome  
&nbsp;&nbsp;&nbsp;&nbsp;• MarkdownLint, YAMLlint  
&nbsp;&nbsp;&nbsp;&nbsp;• PyLint, Hadolint  
✅ Artifact-based build and release strategy  
✅ Manual approval gates for controlled deployments  
✅ VM-based deployment automation using pipeline environments  

> This is a **delivery pipeline**, not a demo pipeline.

---

## 🧩 CI/CD Architecture (Azure DevOps)

**Primary pipeline file:**  
`production-grade-pipeline.yml`

The pipeline is structured to mirror how enterprises enforce **security, governance, and traceability**.

### 🧱 Pipeline Stages

1. **Software Composition Analysis**
   - Dependency vulnerability scanning using Retire.js

2. **Static Code Analysis**
   - Code quality and maintainability checks via SonarQube/SonarCloud

3. **Code Quality & Linting**
   - Frontend, backend, Dockerfile, YAML, and Markdown linting
   - Non-blocking checks to surface issues without halting learning

4. **Build & Artifact Packaging**
   - Frontend build → versioned artifact
   - Backend packaging → deployable artifact

5. **Approval Gate**
   - Manual validation to enforce change control

6. **Deploy to Dev**
   - UI deployed to VM web directory
   - Backend deployed, dependencies installed, and service started

---

## 📦 Deployment Strategy

- CI produces **immutable artifacts**
- CD deploys artifacts using **Azure DevOps Environments**
- Virtual Machines are treated as **controlled delivery targets**
- Deployment logic is separated from build logic

This closely mirrors **enterprise VM-based delivery models** still widely used in production.

---

## 🔐 Security & Governance Notes

- No secrets are committed to the repository
- Credentials are managed via:
  - Azure DevOps Variable Groups
  - Service Connections
- Approval gates ensure accountability and auditability

🔮 **Planned enhancement:**  
OIDC / Federated authentication for password-less Azure access.

---

## 🧭 Design Decisions & Trade-offs

- VM deployments chosen to reflect legacy + hybrid environments
- linting to demonstrate quality enforcement
- Manual approvals included to reflect regulated environments
- Simplicity in application to keep focus on delivery mechanics

---

## 👤 Author

**Bhabya Bharti**  
DevOps Engineer | CI/CD | Terraform | Azure | DevSecOps
