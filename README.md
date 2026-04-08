# 🚀 End-to-End AWS Static Website Deployment  
## From Manual Setup to CI/CD Automation

---

## 📖 Introduction

With several years of experience working with AWS, I have had the opportunity to interact with a wide range of cloud services in different contexts.

However, over time, I realized that mastering AWS is not only about using individual services, but about **designing complete, production-ready systems and being able to clearly demonstrate that expertise**.

This realization led me to start building and documenting my projects as part of a structured portfolio.

This repository is part of that journey — a series of hands-on projects where I focus on:

- building real-world cloud architectures,
- documenting every step clearly,
- and showcasing my ability to design, deploy, and automate scalable systems.

---

## 🎯 Project Overview

This project demonstrates how to deploy a **secure, scalable, and globally distributed static website on AWS**, following real-world practices.

It is structured into two complementary parts:

- **Part 1 — Manual Deployment:** building and deploying the infrastructure step by step using core AWS services.
- **Part 2 — CI/CD Automation:** automating the entire deployment pipeline using GitHub Actions.

The goal is to demonstrate a full progression:

> from manual cloud setup → to automated, production-grade deployment.

---

## 🌍 Live Website

👉 https://soscompany.co  
👉 https://www.soscompany.co  

---

## 🏗️ Global Architecture Overview

![Architecture](./architecture/26-architecture-diagram.png)

This architecture follows a modern cloud pattern:

- Users access the application via a custom domain
- DNS (Namecheap) routes traffic to CloudFront
- CloudFront distributes content globally (low latency)
- AWS Certificate Manager (ACM) provides HTTPS security
- Amazon S3 stores and serves the static website

### ✅ Key Benefits

- High availability  
- Global performance  
- Secure HTTPS communication  
- Scalable and production-ready infrastructure  

---

## ⚙️ Tech Stack

- **Frontend:** HTML, CSS, JavaScript (Vite)
- **Cloud Provider:** AWS
- **Storage:** Amazon S3
- **CDN:** Amazon CloudFront
- **SSL/TLS:** AWS Certificate Manager (ACM)
- **DNS:** Namecheap
- **Version Control:** Git & GitHub
- **Automation:** GitHub Actions *(Part 2)*

---

# 🧩 Part 1 — Manual Deployment on AWS

## 📌 Part 1 Overview

In this first phase, the entire infrastructure is deployed manually in order to fully understand how each AWS component works and how they integrate together in a real-world setup.

Rather than abstracting the process, this step focuses on:

- configuring each service from scratch,
- understanding the underlying mechanisms,
- and troubleshooting real deployment issues.

This approach ensures a solid foundation before moving to automation.

---

## 1️⃣ Local Development & Build

### Project structure
![Step 1](./screenshots/screenshots-projet-1/01-project-structure-local.png)

### Local preview
![Step 2](./screenshots/screenshots-projet-1/02-local-development-preview.png)

### Production build
![Step 3](./screenshots/screenshots-projet-1/03-production-build-dist-folder.png)

---

## 2️⃣ GitHub Repository Setup

### Repository created
![Step 4](./screenshots/screenshots-projet-1/04-github-repository-created.png)

### Project structure on GitHub
![Step 5](./screenshots/screenshots-projet-1/05-github-project-structure.png)

---

## 3️⃣ Amazon S3 Setup

### Bucket creation
![Step 6](./screenshots/screenshots-projet-1/06-s3-bucket-created.png)

### Files uploaded
![Step 7](./screenshots/screenshots-projet-1/07-s3-files-uploaded.png)

### Static hosting enabled
![Step 8-1](./screenshots/screenshots-projet-1/08-s3-static-hosting-enabled-1.png)
![Step 8-2](./screenshots/screenshots-projet-1/08-s3-static-hosting-enabled-2.png)

### First test (before permissions)
![Step 9](./screenshots/screenshots-projet-1/09-s3-website-first-test.png)

### Public bucket policy
![Step 10](./screenshots/screenshots-projet-1/10-s3-bucket-policy-public.png)

### Website working from S3 endpoint
![Step 11](./screenshots/screenshots-projet-1/11-s3-website-live.png)

---

## 4️⃣ CloudFront Setup (CDN)

### Get started
![Step 12](./screenshots/screenshots-projet-1/12-cloudfront-get-started.png)

### Origin configuration
![Step 13](./screenshots/screenshots-projet-1/13-cloudfront-origin-configuration.png)

### Security settings
![Step 14](./screenshots/screenshots-projet-1/14-cloudfront-security-settings.png)

### Distribution deploying
![Step 15](./screenshots/screenshots-projet-1/15-cloudfront-distribution-deploying.png)

### CloudFront live
![Step 16](./screenshots/screenshots-projet-1/16-cloudfront-website-live.png)

### Default root object fix
![Step 17](./screenshots/screenshots-projet-1/17-cloudfront-default-root-fixed.png)

---

## 5️⃣ SSL Certificate with ACM

### ACM dashboard
![Step 18](./screenshots/screenshots-projet-1/18-acm-dashboard.png)

### Domain configuration
![Step 19](./screenshots/screenshots-projet-1/19-acm-domain-names.png)

### CNAME records generated by AWS
![Step 20-1](./screenshots/screenshots-projet-1/20-acm-cname-records-1.png)
![Step 20-2](./screenshots/screenshots-projet-1/20-acm-cname-records-2.png)

### DNS validation (Namecheap)
![Step 21](./screenshots/screenshots-projet-1/21-namecheap-acm-validation.png)

### Certificate issued
![Step 22](./screenshots/screenshots-projet-1/22-acm-certificate-issued.png)

---

## 6️⃣ Custom Domain + HTTPS

### CloudFront domain configuration
![Step 23](./screenshots/screenshots-projet-1/23-cloudfront-domain-config.png)

### DNS setup (Namecheap → CloudFront)
![Step 24](./screenshots/screenshots-projet-1/24-dns-namecheap-cloudfront.png)

### Final result (HTTPS working)
![Step 25](./screenshots/screenshots-projet-1/25-final-domain-working.png)

---

## 🔥 Key Features

- ✅ Static website hosting with S3  
- ✅ Global CDN with CloudFront  
- ✅ HTTPS secured with ACM  
- ✅ Custom domain integration  
- ✅ High performance & low latency  
- ✅ Production-ready deployment  

---

## 🧠 Challenges & Solutions

### ❌ S3 Access Denied (403)  
✔️ Fixed by applying a public bucket policy  

### ❌ CloudFront not loading index.html  
✔️ Fixed by setting the Default Root Object  

### ❌ SSL validation stuck  
✔️ Fixed DNS CNAME configuration in Namecheap  

### ❌ Git push rejected  
✔️ Solved using `git pull --rebase`  

---

## 💼 Skills Demonstrated

- AWS S3 configuration  
- CloudFront CDN architecture  
- DNS management (Namecheap)  
- SSL/TLS setup (ACM)  
- Debugging production issues  
- Git & GitHub workflow  
- End-to-end cloud deployment  

---

# 🔄 Next Step — CI/CD Automation

After completing the manual deployment, the next step is to automate the entire workflow using GitHub Actions.

👉 This will be covered in **Part 2**.
