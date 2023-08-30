# AWS-VPC-With-S3

### Problem Statement
![image](https://github.com/andrew-anter/AWS-VPC-With-S3/assets/56892364/7248f8d9-eeca-4ddf-9f40-5e6a29ba87a8)

Implement a VPC with the following specifications:
<ul>
<li>CIDR: 10.0.0.0/16</li>
<li>Two public subnets:<ul>
<li>CIDR: 10.0.0.0/24</li>
<li>CIDR: 10.0.0.2.0/24</li>
</ul></li>
<li>One load balancer to distribute traffic between two machines with nginx installed as a proxy</li>
<li>Two private subnets:<ul>
<li>CIDR: 10.0.1.0/24
<li>CIDR: 10.0.0.3.0/24
</ul></li>
<li>Two EC2 instances attached to an Auto Scaling group in the private subnets with Apache installed without SSH
<li>A load balancer installed between the EC2 instances
<li>The EC2 instances will get the application from an S3 bucket
</ul>

### Solution

The solution is implemented using Terraform, a tool for provisioning infrastructure as code. The Terraform configuration files in this repository create the necessary resources in AWS. The following steps are involved in the solution:

<ol>
<li>Create a VPC with CIDR 10.0.0.0/16.
<li>Create two public subnets with CIDRs 10.0.0.0/24 and 10.0.0.2.0/24.
<li>Create a load balancer and attach it to the public subnets.
<li>Create two private subnets with CIDRs 10.0.1.0/24 and 10.0.0.3.0/24.
<li>Create two EC2 instances in the private subnets and attach them to an Auto Scaling group.
<li>Install Apache on the EC2 instances without SSH.
<li>Install a load balancer between the EC2 instances.
<li>Configure the EC2 instances to get the application from an S3 bucket.
</ol>
  
### Usage

To use this solution, you can follow these steps:

<ol>
<li>Install Terraform.
<li>Clone this repository.
<li>Initialize Terraform.
<li>Plan the deployment.
<li>Apply the deployment.
</ol>
  
### Dependencies

This solution depends on the following Terraform plugins:
<ol>
<li>AWS
<li>S3
</ol>

### Troubleshooting

If you encounter any problems with this solution, you can refer to the following resources:
<ul>
<li>Terraform documentation: https://www.terraform.io/docs/index.html
<li>AWS documentation: https://docs.aws.amazon.com/
</ul>

### Screenshots From My Solution:
https://github.com/andrew-anter/AWS-VPC-With-S3/blob/main/Problem%20Solution.pdf
