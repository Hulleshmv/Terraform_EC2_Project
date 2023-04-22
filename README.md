# Terraform_EC2_Project
create an EC2 instance type t2 micro using terraform
This Terraform script automates the creation of a VPC with two subnets, an Internet Gateway, a route table, and security groups in AWS. 
The script also provisions an EC2 instance in one of the subnets.

Prerequisites:

Before running this script, make sure you have the following:
An AWS account
The AWS CLI installed and configured with your credentials

Terraform installed on your local machine

Clone this repository to your local machine:
git clone https://github.com/your-username/aws-terraform-vpc.git

Change into the cloned directory:
cd aws-terraform-vpc

Initialize the Terraform project:
terraform init

Plan the infrastructure changes:
terraform plan

Apply the infrastructure changes:
terraform apply

Verify that the EC2 instance was created and is running:
terraform show
vpc_cidr_block: The CIDR block for the VPC.
subnet_a_cidr_block: The CIDR block for the first subnet.
subnet_b_cidr_block: The CIDR block for the second subnet.
region: The AWS region where the VPC and resources will be created.
instance_type: The instance type for the EC2 instance.
ami: The ID of the Amazon Machine Image (AMI) to use for the EC2 instance.
key_name: The name of the EC2 key pair to use to connect to the instance.

Outputs:
This Terraform script outputs the following resources:

vpc_id: The ID of the created VPC.
subnet_a_id: The ID of the first subnet.
subnet_b_id: The ID of the second subnet.
internet_gateway_id: The ID of the created Internet Gateway.
route_table_id: The ID of the created route table.
security_group_id: The ID of the created security group.
ec2_instance_id: The ID of the created EC2 instance.
