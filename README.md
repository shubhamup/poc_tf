Web App Infrastructure on AWS using Terraform

**Infrastructure Overview**

Goal: Provision:

An EC2 instance (web server) in a public subnet

An RDS instance (database) in a private subnet

Secure networking (controlled via security groups)

Output key info (EC2 public IP, RDS endpoint)

**Terraform Project Structure**

poc_tf/
├── main.tf
├── variables.tf
├── outputs.tf
├── user_data.sh
├── backend.tf
└── terraform.tfvars

backend.tf – Remote Backend (S3 example)
variables.tf – Input Variables
main.tf – Main Infrastructure Code
user_data.sh – EC2 Configuration Script
outputs.tf – Useful Outputs
terraform.tfvars – Your Custom Inputs

**To provisioning the infa use follow below commands.**

**Initialize Terraform**
terraform init

**Validate & Apply**
terraform plan
terraform apply

**Access EC2**

Visit: http://<ec2_public_ip> to verify the web server

**Clean Up**

terraform destroy


