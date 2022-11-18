# ELB Example

Requirements:
- I have web server and I want to deploy it in a scalable environment 

Steps:
- Create Launch Configuration.
- Create Load Balancer.
- Security Group to enable you to access the ec2 using SHH.
- Created autoscaling group to manage any unplanned traffic. 

Deploy: 
- Upload the templates files except the root on S3 bucket 
- Run `cloudformation -template-file [link-root-template] BucketURLParam=[Bucket-URL-include-child-templates] KeyName=[Pair-key-name]`
![Diagram](./ALB.drawio.png) 