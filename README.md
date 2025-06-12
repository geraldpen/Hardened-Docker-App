

---

### 🔐 Hardened Docker App: Learn Docker Security Step-by-Step

This project demonstrates how to **build a Node.js application with insecure Docker practices**, then gradually **harden it using real-world DevSecOps techniques**.

It’s built for:

* Developers who want to write **more secure Dockerfiles**
* DevOps engineers looking to **apply container security best practices**
* Security professionals exploring **container misconfigurations and mitigations**

---

### 📋 What This Repo Covers

Each commit (and folder) showcases a different stage in the hardening process:

1. **\[backend/]**: The insecure baseline (`latest`, runs as root, no scanning)
2. **\[hardened-base/]**: Uses specific Node version, non-root user
3. **\[secure-build/]**: Minimal base image, multi-stage build
4. **\[scanning/]**: Vulnerability scans using Trivy and Grype
5. **\[secrets-management/]**: Safe handling of environment variables
6. **\[runtime-hardening/]**: AppArmor, seccomp, read-only FS, and more
7. **\[signed-images/]**: Image signing & verification with `cosign`
8. **\[compliance/]**: Docker Bench Security and CIS checks

---
Getting Started

```bash
git clone https://github.com/geraldpen/Hardened-Docker-App.git
cd docker-hardening backend
docker build -t  backend .
docker run -p 3000:3000 backend
```

Then follow each step in the series as we secure the container image. 

---

###  Blog/Series

This project is part of a **LinkedIn content series** by mokom Gerald penn, a DevSecOps engineer focused on container, wep applcation security and cloud security.
Follow the journey 👉 https://www.linkedin.com/in/mokom-gerald-penn-15b0b3214?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app

---

### 🛠️ Tools Used

* Docker
* Node.js
* Trivy
* Grype
* Docker Bench for Security
* Cosign
* AppArmor / Seccomp

---

### 🤝 Contributions Welcome

Want to try securing it your way? Open a PR or raise an issue.

---

