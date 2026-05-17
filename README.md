# ☁️ AWS Infrastructure Provisioning with Terraform (S3 Bucket)

This repository contains the Terraform configuration to automatically provision an Amazon S3 bucket on AWS. This project demonstrates the core concepts of **Infrastructure as Code (IaC)**, automation, and cloud resource management.

---

## 🎯 Project Overview
The goal of this project is to move away from manual AWS Console configuration ("ClickOps") and adopt a repeatable, automated approach to managing cloud infrastructure. 

During the initial deployment, an authorization and region mismatch error (`AuthorizationHeaderMalformed`) was encountered because the AWS Account root was bound to the Tokyo (`ap-northeast-1`) region, while the initial script target was `us-east-1`. The provider configuration was successfully refactored and debugged to achieve a successful deployment.

---

## 🛠️ Tech Stack & Tools
* **Infrastructure as Code (IaC):** Terraform (v1.15.3)
* **Cloud Provider:** Amazon Web Services (AWS)
* **Core Service:** Amazon S3 (Simple Storage Service)
* **IDE:** Visual Studio Code
* **Shell Environment:** PowerShell / VS Code Terminal

---

## 📂 Code Configuration (`main.tf`)
The infrastructure is defined using declarative HCL (HashiCorp Configuration Language) targeting the `ap-northeast-1` region for resource creation:



    Environment = "Dev"
  }
}
