# TerraformAWS
Exploratory project on understanding Terraform. 

Builds a webserver by standing up the following on ECS-AWS:

1. Provision a provider using AWS

2. Provision a VPC resource (holds all our route table information)

3. Create an internet gateway for us to access the actual website

4. Create a subnet that divides our vpc and associates with the route table

5. Create a route table that builds based off our VPC.id and opens all ipv4 and ipv6 routes

6. Create a security group to allow web traffic (HTTPS, HTTP, SSL)

7. Create the network interface that connects the subnet and the security groups into one

8. Create an AWS EIP (elastic ip address) that connects to the private IP made in our network interface

9. Create the AWS instance and install apache2
