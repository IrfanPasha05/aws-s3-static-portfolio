🌐 AWS S3 Static Portfolio Website

This project demonstrates how to host a static portfolio website on Amazon S3 using secure IAM access and proper public access configuration.

It focuses on real-world AWS fundamentals such as S3 static hosting, IAM least-privilege permissions, bucket policies, and troubleshooting access issues.

🚀 Live Website

👉 (Add your S3 static website endpoint here)
Example:

http://<your-bucket-name>.s3-website-us-east-1.amazonaws.com

📸 Screenshot

👉 (Add a screenshot of the working website inside a screenshots/ folder and link it here)

screenshots/s3-website-working.png

🛠️ Tech Stack

Amazon S3 – Static Website Hosting

AWS IAM – Secure access management

HTML & CSS – Website content and styling

Git & GitHub – Version control

📁 Project Structure
aws-s3-static-portfolio/
├── index.html
├── assets/
│   └── profile.png
├── screenshots/
│   └── s3-website-working.png
└── README.md

🧱 Project Workflow
1️⃣ S3 Bucket Setup

Created a globally unique S3 bucket

Disabled Block all public access

Enabled Static website hosting

Configured index.html as the entry point

2️⃣ Public Access Configuration

Applied a bucket policy to allow public read access to website objects

Ensured access was limited only to required resources

3️⃣ IAM Security (Least Privilege)

Created a dedicated IAM user

Avoided root account usage

Granted only S3-specific permissions

Resolved permission issues like:

s3:ListAllMyBuckets

4️⃣ Deployment

Uploaded static files to S3

Verified website access via browser

Fixed broken asset paths and image loading issues

🔐 Security Best Practices Followed

✅ No root account usage for daily tasks

✅ IAM user with limited permissions

✅ Explicit bucket policy for public access

✅ Least-privilege access model

📌 Key Learnings

IAM users have no permissions by default

Static website hosting still requires explicit public access

s3:ListAllMyBuckets is required for S3 console visibility

S3 object paths are case-sensitive

Bucket policies play a critical role in public access

📦 Future Improvements

Add CloudFront for HTTPS and caching

Attach a custom domain using Route 53

Improve UI and responsiveness

Automate deployment using CI/CD

👤 Author

Irfan Pasha
AWS & DevOps Enthusiast

Dev--https://dev.to/irfanpasha/hosting-a-static-portfolio-website-on-aws-s3-using-iam-beginner-project-3ao4

