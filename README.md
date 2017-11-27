# AWS-tutorial
## 1. Installing R Studio Server on EC2 Server
## 2. Creation of public and private subnet in a VPC with internet connections (Jumpbox)

### 2.1 Steps
1. Create VPC
2. Create 2 subnets
3. Create Internet Gateway and attach to VPC
4. Create a routing table for public subnet.
5. Associate the subnet and add route using the internet Gateway to all IPs over the internet (0.0.0.0/0)
6. Create NAT Gateway and associate it with Public Subnet and attach an EIP
7. Make a routing table for private subnet, associate, add route to 0.0.0.0/0 with target as the NAT gateway you created
8. Make 2 instances and assign to each subnet
9. SSH to the public subnet using Putty
10. Create a file with pem extension and CAT the contents of the public key from your local machine. Save it.
11. Change the permissions to 400 using CHMOD
12. Use it to SSH to private instance.
13. Ping to google.com to check if the instance can access the internet.
