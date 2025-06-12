# 🚀 Securing S3 Bucket with Terraform

This project provisions a secure, versioned, and encrypted AWS S3 bucket using [Terraform](https://www.terraform.io/) following cloud security and compliance best practices including encryption at rest, object versioning, and blocking public access by default.

---

## 🔐 Features

- ✅ AES-256 encryption 
- ✅ Versioning for object recovery
- ✅ Public access blocked

---
## 📂 Repo Structure

```
secure-s3-terraform/
├── .gitignore
├── README.md        ← You are here!
├── main.tf
├── outputs.tf
├── variables.tf
```
---
## 🧰 Prerequisites

Before you begin, make sure you have:

- [Terraform installed](https://developer.hashicorp.com/terraform/install)
- AWS credentials configured via `aws configure`
- An IAM user with permissions to create S3 resources

---

## 🧱 Initialize and Deploy

```bash
terraform init
terraform plan
terraform apply
```
---

## 🧹 Destroy Resources (Cleanup)

```bash
terraform destroy
```

---

## 📜 SOC 2 Compliance Mapping

This Terraform project helps support the following SOC 2 Common Criteria:

| SOC 2 Control | Description |
|---------------|-------------|
| **CC6.1** – Logical Access Controls | Public access to the S3 bucket is blocked to prevent unauthorized access |
| **CC6.6** – Encryption & Confidentiality | AES-256 encryption at rest ensures stored data remains confidential |
| **CC7.1** – Change Management | Terraform enables version-controlled, auditable infrastructure changes |
| **CC8.1** – Data Retention & Disposal | Versioning supports secure data lifecycle management and recovery |
