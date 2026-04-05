# 🚀 AWS Static Website Deployment (S3 + CloudFront + ACM + Custom Domain)

## 🌐 Live Demo

👉 https://soscompany.co  
👉 https://www.soscompany.co  

---

## 📖 Story Behind This Project

When I started learning AWS, deploying a real-world application felt complex and overwhelming.

Instead of just following tutorials, I decided to build a complete production-ready project from scratch something that reflects real industry practices.

This project demonstrates my ability to:

- Deploy a static website using AWS
- Configure a global CDN with CloudFront
- Secure the application using HTTPS (ACM)
- Connect and manage a real custom domain

During this project, I faced real-world challenges such as:

- ❌ S3 Access Denied errors
- ❌ DNS misconfiguration issues
- ❌ SSL validation delays

And I successfully diagnosed and resolved each of them.

👉 This is not just a tutorial project — it is a real deployment scenario.

---

## 🏗️ Architecture Overview

![Architecture](./architecture/26-architecture-diagram.png)

---

## 🎯 Project Overview

This project demonstrates the deployment of a **production-ready static website** using AWS services.

The goal was to build a **scalable, secure, and globally distributed web application** using:

- Amazon S3 (static hosting)
- Amazon CloudFront (CDN)
- AWS Certificate Manager (SSL/TLS)
- Custom domain via Namecheap

---

## ⚙️ Tech Stack

- **Frontend**: HTML, CSS, JavaScript (Vite build)
- **Cloud Provider**: AWS
- **Storage**: Amazon S3
- **CDN**: Amazon CloudFront
- **SSL**: AWS Certificate Manager (ACM)
- **DNS**: Namecheap

---

# 🧩 Step-by-Step Deployment

---

## 1️⃣ Local Development & Build

### Project structure
![Step 1](./screenshots/01-project-structure-local.png)

### Local preview
![Step 2](./screenshots/02-local-development-preview.png)

### Production build
![Step 3](./screenshots/03-production-build-dist-folder.png)

---

## 2️⃣ GitHub Repository Setup

### Repository created
![Step 4](./screenshots/04-github-repository-created.png)

### Project structure on GitHub
![Step 5](./screenshots/05-github-project-structure.png)

---

## 3️⃣ Amazon S3 Setup

### Bucket creation
![Step 6](./screenshots/06-s3-bucket-created.png)

### Files uploaded
![Step 7](./screenshots/07-s3-files-uploaded.png)

### Static hosting enabled
![Step 8](./screenshots/08-s3-static-hosting-enabled-1.png)
![Step 8](./screenshots/08-s3-static-hosting-enabled-2.png)

### First test (before permissions)
![Step 9](./screenshots/09-s3-website-first-test.png)

### Public bucket policy
![Step 10](./screenshots/10-s3-bucket-policy-public.png)

### Website working (S3 endpoint)
![Step 11](./screenshots/11-s3-website-live.png)

---

## 4️⃣ CloudFront (CDN Setup)

### Get started
![Step 12](./screenshots/12-cloudfront-get-started.png)

### Origin configuration
![Step 13](./screenshots/13-cloudfront-origin-configuration.png)

### Security settings
![Step 14](./screenshots/14-cloudfront-security-settings.png)

### Distribution deploying
![Step 15](./screenshots/15-cloudfront-distribution-deploying.png)

### CloudFront live
![Step 16](./screenshots/16-cloudfront-website-live.png)

### Default root object fix
![Step 17](./screenshots/17-cloudfront-default-root-fixed.png)

---

## 5️⃣ SSL Certificate (ACM)

### ACM Dashboard
![Step 18](./screenshots/18-acm-dashboard.png)

### Domain configuration
![Step 19](./screenshots/19-acm-domain-names.png)

### CNAME records (AWS)
![Step 20](./screenshots/20-acm-cname-records-1.png)
![Step 20](./screenshots/20-acm-cname-records-2.png)

### DNS validation (Namecheap)
![Step 21](./screenshots/21-namecheap-acm-validation.png)

### Certificate issued
![Step 22](./screenshots/22-acm-certificate-issued.png)

---

## 6️⃣ Custom Domain + HTTPS

### CloudFront domain configuration
![Step 23](./screenshots/23-cloudfront-domain-config.png)

### DNS setup (Namecheap → CloudFront)
![Step 24](./screenshots/24-dns-namecheap-cloudfront.png)

### Final result (HTTPS working)
![Step 25](./screenshots/25-final-domain-working.png)

---

# 🔥 Key Features

- ✅ Static website hosting with S3  
- ✅ Global CDN with CloudFront  
- ✅ HTTPS secured with ACM  
- ✅ Custom domain integration  
- ✅ High performance & low latency  
- ✅ Production-ready deployment  

---

# 🧠 Challenges & Solutions

### ❌ S3 Access Denied (403)
✔️ Fixed by applying a public bucket policy

### ❌ CloudFront not loading index.html
✔️ Fixed by setting **Default Root Object**

### ❌ SSL validation stuck
✔️ Fixed DNS CNAME configuration in Namecheap

### ❌ Git push rejected
✔️ Solved using `git pull --rebase`

---

# 💼 Skills Demonstrated

- AWS S3 configuration
- CDN architecture (CloudFront)
- DNS management (Namecheap)
- SSL/TLS setup (ACM)
- Debugging production issues
- Git & GitHub workflow
- End-to-end cloud deployment

---

# 🚀 Future Improvements

- CI/CD pipeline (GitHub Actions)
- Infrastructure as Code (Terraform)
- Monitoring (CloudWatch)
- Logging & alerting
- Route 53 integration
- WAF security layer

---

# 📌 What I learned

This project demonstrates the ability to design and deploy a **secure, scalable, and production-ready web architecture on AWS**.

It highlights real-world problem-solving, cloud best practices, and DevOps fundamentals.

---

# 👨‍💻 Author

**Dassaev TCHOUTA**  
Cloud / DevOps Enthusiast 🚀
