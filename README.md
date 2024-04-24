# Static Website Hosting on AWS S3

## Overview
This guide provides steps to host a static website on Amazon S3. By following these steps, you can create a scalable and reliable website that can handle high levels of traffic.

## S3 Bucket Set Up
1. Open S3 on a separate tab.
2. Click on "Create Bucket".
3. Enter the following information: Bucket Name="any globally unique name or MyStaticWebsite123456", AWS Region="choose closest to country you'll be using it or choose US-East-1 as default".
4. Under "Block public access (bucket settings)", uncheck all options.
5. Leave default settings, and click on "Create bucket".
6. Under "Buckets", choose "Properties".
7. Under "Static website hosting", click "Edit".
8. Under "Static website hosting", choose "Enable".
9. Under "Hosting type", choose "Host static website".
10. Under "Index", type "index.html".
11. Leave default settings, and click on "Save changes".
12. Under "Buckets", choose "Permission".
13. Under "Bucket Policy", click "Edit".
14. Enter JSON attached to this project.
15. Change "arn:aws:s3:::Bucket-Name/*" for the Bucket ARN at the top of the screen.
16. Click on "Save changes".
17. Under "Buckets", choose "Object".
18. Upload your index.html file and any images, and click "Upload".
19. Under "Static website hosting", click on url below "Bucket website endpoint".

## Clean Up
Empty and terminate S3 Bucket (e.g. you may need to delete bucket policy). To avoid unnecessary costs, please double-check that no underlying resources are still running.

## Conclusion
In this project, we demonstrated how to host a static website on AWS S3. By following these steps, we have created a scalable and reliable website that can handle high levels of traffic. Feel free to message me with code improvement suggestions.

## Acknowledgment
This tutorial is adapted from the [AWS S3 tutorial for hosting a static website](https://docs.aws.amazon.com/AmazonS3/latest/userguide/HostingWebsiteOnS3Setup.html) provided by Amazon Web Services. We extend our gratitude to AWS for providing this valuable resource, which served as the foundation for the "Static Website Hosting on AWS S3" tutorial.
