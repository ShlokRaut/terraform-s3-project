# AWS Infrastructure Deployment using Terraform (S3 Bucket Automation)

**Author:** Shloka  
**Email:** shlokraut01@gmail.com  

---

## Project Overview

This project demonstrates my ability to design and deploy cloud infrastructure on AWS using Infrastructure as Code (Terraform). I implemented an automated workflow to provision and manage an Amazon S3 bucket.

Instead of manually creating resources through the AWS console, I used Terraform configuration files to define and deploy infrastructure consistently and efficiently.

---

## What I Built

In this project, I:

- Installed and configured Terraform  
- Set up AWS credentials using AWS CLI  
- Defined infrastructure using Terraform configuration files (`main.tf`)  
- Created an AWS S3 bucket using Terraform  
- Uploaded and managed objects in S3 using Infrastructure as Code  
- Applied Terraform workflow: `init`, `plan`, `apply`, `destroy`  

---

## Tools & Technologies

- Terraform (Infrastructure as Code)
- AWS S3 (Cloud Storage)
- AWS IAM (Access Management)
- AWS CLI
- Git & GitHub

---

## Key Concepts Learned

- Infrastructure as Code (IaC)
- Cloud resource provisioning using Terraform
- AWS authentication using access keys
- Terraform workflow and state management
- Automating cloud infrastructure deployment

---

## Terraform Workflow

- `terraform init` → Initializes project and downloads providers  
- `terraform plan` → Shows execution plan  
- `terraform apply` → Creates infrastructure in AWS  
- `terraform destroy` → Removes infrastructure  

---

## Project Outcome

Successfully deployed an AWS S3 bucket using Terraform and verified the deployment through the AWS Management Console.

---

## Key Takeaway

This project strengthened my understanding of cloud infrastructure automation and real-world DevOps practices using Terraform and AWS.
I added a new resource block to define an additional AWS resource (an S3 object), allowing Terraform to manage and create it automatically within my existing infrastructure.

We need to run `terraform apply` again because the configuration was updated, and Terraform must apply the new desired state to AWS.

I validated the upload by checking the AWS S3 console and confirming that the file appeared in the correct bucket after running `terraform apply`.
