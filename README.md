# 🚀 Terraform AWS EC2 Instance

This project uses Terraform to provision a secure Amazon EC2 instance on AWS.

---

## 🛠️ Features

- AWS provider configuration using variables
- Uploads your local SSH public key as a key pair
- Creates a security group allowing inbound SSH (port 22)
- Launches a `t2.micro` Amazon Linux 2 instance
- Outputs public IP for easy connection

---

## 🧾 Files

| File              | Description                         |
|-------------------|-------------------------------------|
| `main.tf`         | Main Terraform configuration        |
| `variables.tf`    | Input variables for flexibility     |
| `terraform.tfvars`| Actual values for variables (ignored in Git) |
| `outputs.tf`      | Public IP output                    |
| `.gitignore`      | Ensures secrets/state aren’t committed |

---

## ⚙️ Usage

```bash
terraform init
terraform plan
terraform apply
