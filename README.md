AWS Static Website Deployment (S3 + CloudFront + Custom Domain + HTTPS)

 Project Overview

This project demonstrates a **production-ready deployment of a static website on AWS**, using industry best practices.

The architecture includes:

* **Amazon S3** for static website hosting
* **Amazon CloudFront** as a CDN (Content Delivery Network)
* **AWS Certificate Manager (ACM)** for HTTPS (SSL/TLS)
* **Custom domain (Namecheap)** for public access
* **DNS configuration** for domain routing

---

## 🌍 Live Website

🔗 https://soscompany.co
🔗 https://www.soscompany.co

---

## 🏗️ Architecture Overview

* Static files are hosted in an S3 bucket
* CloudFront distributes content globally with caching
* ACM provides a secure SSL certificate (HTTPS)
* Namecheap DNS connects the domain to CloudFront

---

## 📸 Project Walkthrough (Step-by-Step)

### 🖥️ Local Development

* 01-project-structure-local.png
* 02-local-development-preview.png
* 03-production-build-dist-folder.png

---

### 🐙 GitHub Repository Setup

* 04-github-repository-created.png
* 05-github-project-structure.png

---

### ☁️ Amazon S3 Configuration

* 06-s3-bucket-created.png
* 07-s3-files-uploaded.png
* 08-s3-static-hosting-enabled.png
* 08-s3-static-hosting-enabled-2.png
* 09-s3-website-first-test.png
* 10-s3-bucket-policy-public.png
* 11-s3-website-live.png

---

### 🌐 CloudFront Setup

* 12-cloudfront-get-started.png
* 13-cloudfront-origin-configuration.png
* 14-cloudfront-security-settings.png
* 15-cloudfront-distribution-deploying.png
* 16-cloudfront-website-live.png
* 17-cloudfront-default-root-fixed.png
* 23-cloudfront-domain-config.png

---

### 🔐 SSL Certificate (ACM)

* 18-acm-dashboard.png
* 19-acm-domain-names.png
* 20-acm-cname-records-1.png
* 20-acm-cname-records-2.png
* 21-namecheap-acm-validation.png
* 22-acm-certificate-issued.png

---

### 🌍 DNS Configuration (Namecheap)

* 24-dns-namecheap-cloudfront.png

---

### 🎉 Final Result

* 25-final-domain-working.png

---

## ⚙️ Technologies Used

* Amazon S3
* Amazon CloudFront
* AWS Certificate Manager (ACM)
* Namecheap DNS
* Git & GitHub

---

## 🔐 Key Features Implemented

* Static website hosting on S3
* Global CDN distribution with CloudFront
* HTTPS secured website using ACM
* Custom domain integration
* DNS configuration via Namecheap
* Public access configuration via bucket policy
* Default root object handling (index.html)

---

## 🧠 Key Learnings

* How to deploy a static website on AWS
* How to configure CloudFront for performance and security
* How to issue and validate SSL certificates with ACM
* How DNS works with external providers (Namecheap)
* How to connect a custom domain to AWS infrastructure
* Understanding caching and CDN behavior

---

## ⚠️ Challenges Faced & Solutions

### ❌ 403 Forbidden Error (S3)

✔️ Fixed by configuring correct bucket policy and public access

### ❌ Domain not resolving

✔️ Fixed by properly configuring CNAME records in Namecheap

### ❌ SSL Validation delay

✔️ Resolved by correcting CNAME host format for subdomain

### ❌ CloudFront default root issue

✔️ Fixed by setting `index.html` as default root object


## 💡 Best Practices Applied

* Separation between origin (S3) and distribution (CloudFront)
* Secure HTTPS configuration
* CDN optimization for performance
* Clean GitHub structure for documentation
* Step-by-step deployment tracking with screenshots

---

## 🚀 Future Improvements

* CI/CD pipeline using GitHub Actions
* Route 53 integration
* Custom error pages (404 / 403)
* Infrastructure as Code (Terraform or CloudFormation)

---

## 👨‍💻 Author

Cloud & DevOps Enthusiast
AWS-focused projects for real-world deployment scenarios

---

## 📌 Summary

This project demonstrates the ability to:

✔ Deploy scalable static websites
✔ Configure CDN and HTTPS
✔ Manage DNS and domains
✔ Work with core AWS services

👉 This is a **real-world production-ready setup** suitable for modern web applications.
