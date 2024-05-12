# AWS S3 Static Website Deployment with Route 53
## Overview
This project demonstrates how to deploy a static website using Amazon S3 and configure domain routing with Amazon Route 53. The website showcases a simple static site built with HTML, CSS, and JavaScript.
## Prerequisites
- An AWS account with permissions to create S3 buckets and configure Route 53
- Basic knowledge of AWS services such as S3 and Route 53
- A registered domain name for configuring domain routing
- ## Setup Instructions
1. Go into Route 53 Console and purchase a domain name under the "Registered Domains" section
2. Create an S3 bucket for your static website using the AWS Management Console.
3. Create a Bucket name that matches the domain name in order for this to properly work.
4. Uncheck "Block public access" so users can publicly access the website.
5. Upload your website files to the S3 bucket then enable static website hosting under "Properties" tab.
6. Enable static website hosting on the S3 bucket and specify the index document.
7. Configure bucket policies by adding your own bucket policy.
8. Verify the website deployment by accessing the website URL.
9. To properly redirect access to the domain website, Go to route 53 and click on "Hosted Zone"
10. Add a new record under "Simple routing policy"
11. Define your simple record in the "selecting Route/Route traffic" section and choosing "Alias to S3 website endpoint"
12. Underneath, select the region in which your bucket was created
13. At the end, select your s3's endpoint and "define simple record" to complete task.
14. Enter your domain website to view your completed project!
## Demo
- [Live Demo](http://xavierproject.click/)

## Troubleshooting
- If you encounter permissions errors when accessing the website, check the bucket policies and ensure public access is allowed.
- If the domain routing is not working as expected, verify the DNS settings in Route 53 and ensure the domain is correctly configured.





