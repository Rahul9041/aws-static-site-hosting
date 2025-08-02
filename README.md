# aws-static-site-hosting
Static Website Hosting using AWS S3, CloudFront, Route 53, and ACM
# 🌐 Static Website Hosting using AWS S3 + CloudFront

This project demonstrates how to host a fully static website on AWS using S3, CloudFront, Route 53, and ACM (SSL Certificate).

---

## 📌 Features

- Website hosted on S3 with public read access
- Distributed via CloudFront CDN for global performance
- HTTPS enabled using AWS Certificate Manager (ACM)
- Custom domain configuration using Route 53

---

## 🧰 Tools & Services Used

- AWS S3 (for static hosting)
- AWS CloudFront (CDN)
- AWS ACM (SSL/TLS)
- AWS Route 53 (DNS & domain management)
- HTML, CSS

---

## 🏗️ Architecture
[User] --> [CloudFront] --> [S3 Bucket (Website Files)]
│
[ACM Certificate + HTTPS]
│
[Custom Domain via Route 53]


---

## 🚀 Steps to Deploy

1. **Create S3 Bucket** (enable static website hosting)
2. **Upload `index.html` and `error.html`**
3. **Create CloudFront Distribution**
   - Origin: S3 bucket website endpoint
   - Enable redirect HTTP → HTTPS
4. **Request ACM Certificate**
   - Validate via DNS in Route 53
5. **Map Domain in Route 53**
   - Add A record (alias to CloudFront)
6. ✅ Website goes live on `https://www.yourdomain.com`

---



---

## 🙋‍♂️ Author

- 👨‍💻 [Rahul Paul](https://www.linkedin.com/in/rahul-paul-2a634b222)
- 📧 rahul9041@gmail.com

---

> This project is part of my DevOps portfolio. Feel free to explore, fork, and connect!


