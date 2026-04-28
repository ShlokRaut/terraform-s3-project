
# Create S3 Buckets with Terraform


**Author:** Shloka  
**Email:** shlokraut01@gmail.com

---



---

## Introducing Today's Project!

In this project, I demonstrate how to use Terraform to automate the creation and management of cloud infrastructure on Amazon Web Services (AWS).

The goal is to provision an Amazon S3 bucket using Infrastructure as Code (IaC), instead of manually creating resources through the AWS console.

By the end of this project, I will:
- Install and configure Terraform  
- Set up AWS credentials securely using the CLI  
- Write Terraform configuration files to define infrastructure  
- Deploy and manage an S3 bucket using Terraform  
- Upload files to the bucket through Terraform automation  

This project highlights how automation improves efficiency, consistency, and scalability in modern cloud environments, which is essential for roles like DevOps and Platform Engineering.

---

## Tools and Concepts

I used Terraform to manage infrastructure as code and deployed an AWS S3 bucket.

Key concepts I learned include:
- Infrastructure as Code (IaC)  
- Terraform workflow (init, plan, apply, destroy)  
- AWS IAM authentication using access keys  
- AWS S3 bucket creation and management  
- Permissions and security in AWS IAM  
- Deploying cloud resources using CLI instead of the console  

---

## Project Reflection

It took me around 1–2 hours to complete this project, including setting up Terraform, configuring AWS CLI, and deploying the S3 bucket.

I chose to do this project today because I wanted to learn how Terraform and AWS work together in real cloud infrastructure setups and gain hands-on experience with Infrastructure as Code.

Something that would make learning with NextWork even better is more step-by-step troubleshooting tips and real-world examples of common errors, so beginners can understand and resolve issues faster when something goes wrong.

---

## Introducing Terraform

Terraform is a tool used to manage AWS infrastructure using code.

Terraform is one of the most popular Infrastructure as Code (IaC) tools, which is a method of managing and provisioning cloud infrastructure using code instead of manual configuration through a web console.

Terraform uses configuration files (like `main.tf`) to define infrastructure.

---

## Configuration Files

My configuration is defined in Terraform using a `.tf` file (such as `main.tf`), where infrastructure is written as code.

The three main blocks describe:

- **Provider block** → specifies the cloud provider (AWS) and region  
- **Resource block (S3 bucket)** → creates the AWS S3 bucket  
- **Resource block (S3 object/file)** → uploads a file into the bucket and manages it through Terraform  

---

## Customizing My S3 Bucket

In the official Terraform documentation, I explored guides and examples that explain how Terraform works, including providers, resources, and commands like `init`, `plan`, `apply`, and `destroy`.

My bucket name: `shlok2999929999`

---

## Terraform Commands

- `terraform init` → sets up the working directory and downloads required provider plugins  
- `terraform plan` → shows a preview of changes before applying them  

---

## AWS CLI and Access Keys

I got an error because my AWS credentials or permissions were not set up correctly, so Terraform could not access AWS resources.

The AWS CLI (Command Line Interface) allows me to manage AWS services using terminal commands instead of the web console.

I set up access keys so the AWS CLI could securely connect to my AWS account and run commands from my terminal.

---

## Launching the S3 Bucket

I ran `terraform apply` to execute the Terraform configuration and create the resources defined in my code (such as an S3 bucket) in my AWS account.

Running `terraform apply` updates my AWS account by provisioning, modifying, or deleting resources based on my Terraform configuration.

The sequence:
- `terraform init` → setup  
- `terraform plan` → preview  
- `terraform apply` → create  
- `terraform destroy` → delete  

This workflow is important because it ensures infrastructure changes are planned, reviewed, and applied consistently.

---

## Uploading an S3 Object

I added a new resource block to define an additional AWS resource (an S3 object), allowing Terraform to manage and create it automatically within my existing infrastructure.

We need to run `terraform apply` again because the configuration was updated, and Terraform must apply the new desired state to AWS.

I validated the upload by checking the AWS S3 console and confirming that the file appeared in the correct bucket after running `terraform apply`.