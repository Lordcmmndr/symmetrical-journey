# symmetrical-journey
First look at AWS S3 Bucket
# Host a Website on Amazon S3

This repository outlines the steps for hosting a static website on Amazon S3, a powerful cloud storage service provided by AWS.

## About Amazon S3
Amazon S3 (Simple Storage Service) is a highly scalable, secure, and durable cloud storage solution. It enables individuals and organizations to store and retrieve any amount of data at any time. S3 also offers features like:
- Static website hosting
- Content delivery

## Project Overview
This project demonstrates how to:
1. Set up an Amazon S3 bucket.
2. Upload website files (HTML and assets).
3. Enable static website hosting.
4. Resolve access errors to make the website publicly accessible.

### Steps to Host a Website on S3

#### 1. Create an S3 Bucket
- Navigate to the AWS S3 Console.
- Create a new bucket. Note that bucket names are globally unique and must adhere to AWS naming conventions.
- Select a region close to your location for optimal performance. For this project, the `eu-north-1` (Stockholm) region was used.

#### 2. Upload Website Files
- Upload the necessary files to the S3 bucket, including:
  - `index.html`: The main HTML file for the website.
  - Image and asset folder: Contains images and other assets for the website.

#### 3. Enable Static Website Hosting
- Go to the "Properties" tab of your S3 bucket.
- Edit the "Static website hosting" option and enable it.
- Specify the `index.html` file as the entry point.

#### 4. Configure Object Permissions
- By default, objects in S3 buckets are private. To make them publicly accessible:
  - Select the uploaded files (e.g., `index.html` and the asset folder).
  - Click on "Actions" > "Make Public".

#### 5. Access Your Website
- Once static website hosting is enabled, AWS provides a bucket endpoint URL.
- Use this URL to access your website. For example: `http://<bucket-name>.s3-website.<region>.amazonaws.com`

### Common Issues
- **403 Forbidden Error**: This occurs when objects are not publicly accessible. Ensure that all website files have public read permissions.

### Time Taken
- Setting up the S3 bucket: ~15 minutes.
- Configuring static hosting and resolving errors: ~45 minutes.

### Additional Resources
- [My NextWork Portfolio](https://community.nextwork.org/c/i-have-a-question?automatic_login=true)
- [AWS S3 Documentation](https://aws.amazon.com/s3/documentation/)
- [NextWork Community](https://community.nextwork.org/c/i-have-a-question?automatic_login=true)

---

#### About the Author
This project was created by **Michael Emeruwa**, a student at NextWork.org, as part of a hands-on learning experience.

"Everyone should be in a job they love." Check out [NextWork.org](https://nextwork.org) for more projects and resources.
