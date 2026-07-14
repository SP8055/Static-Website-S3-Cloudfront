Static Website Hosting on AWS S3 + CloudFront
This project demonstrates how to host a static website using Amazon S3 and serve it securely through Amazon CloudFront with HTTPS enabled.

🚀 Project Overview
S3 Bucket: Stores static website files (index.html, style.css)

CloudFront: CDN for fast global delivery

ACM SSL Certificate: Enables HTTPS (must be requested in us-east-1)

Route 53 (Optional): Custom domain mapping

📂 Project Structure
Code
.
├── index.html
├── style.css
🔧 Deployment Steps
Create an S3 bucket

Enable static website hosting

Upload index.html and style.css

Request SSL certificate in ACM

Must be in us-east-1 region

Validate via DNS or email

Create CloudFront distribution

Set S3 bucket as origin with Origin Access Control (OAC)

Attach ACM SSL certificate

Configure caching and error pages

Update S3 bucket policy

Allow access only from CloudFront

Block direct public access

(Optional) Configure Route 53

Create an alias record pointing your domain to CloudFront

✅ Features
Secure HTTPS delivery

Global CDN with low latency

Locked-down S3 bucket (only CloudFront access)

Simple static site with HTML + CSS

📺 Reference
I followed this tutorial for hands-on setup:
Static Website on S3 + CloudFront (YouTube)

🛠️ Technologies Used
AWS S3

AWS CloudFront

AWS Certificate Manager (ACM)

HTML5, CSS3
