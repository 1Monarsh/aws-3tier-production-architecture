# AWS Three-Tier Production Architecture (Terraform)

A highly available **three-tier AWS architecture** built using Infrastructure as Code with Terraform.
This project demonstrates how to design and deploy a scalable cloud application using core AWS services.
The architecture separates the application into **presentation, application, and data layers**, improving scalability, security, and maintainability.

---

## Architecture Overview

The infrastructure provisions a production-style architecture consisting of:

Internet → Application Load Balancer → Auto Scaling EC2 → RDS Database

The system is deployed inside a custom VPC with public and private subnets.

---

## AWS Services Used

Core services used in this architecture include:

• Amazon VPC – isolated network environment
• Application Load Balancer – distributes incoming traffic
• Amazon EC2 – compute instances running the application
• EC2 Auto Scaling – ensures high availability and scalability
• Amazon RDS – managed relational database
• Internet Gateway – enables internet connectivity
• Security Groups – network level security

---

## Infrastructure as Code

All infrastructure is defined using **Terraform**, allowing the entire environment to be deployed reproducibly.

Key Terraform components:

providers.tf – AWS provider configuration
versions.tf – Terraform version requirements
variables.tf – reusable infrastructure variables
main.tf – core infrastructure resources

---

## Key Features

High availability architecture
Auto-scaling compute layer
Load balanced traffic distribution
Secure database tier
Infrastructure fully defined as code

---

## Architecture Diagram
<img width="1408" height="768" alt="Architecture Daigram" src="https://github.com/user-attachments/assets/8635580d-02ff-461b-9421-8e9290710479" />



---

## Project Structure

```
aws-3tier-production-architecture
│
├── main.tf
├── providers.tf
├── variables.tf
├── versions.tf
├── README.md
└── LICENSE
```

---

## What This Project Demonstrates

This project demonstrates practical experience with:

• AWS networking and VPC design
• Load balancing and traffic distribution
• Auto scaling infrastructure
• Managed databases
• Infrastructure as Code with Terraform

---

## License

MIT License

