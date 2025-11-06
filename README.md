<!-- PROJECT HEADER -->
<h1 align="center">🚀 JOVAC – Multi-Cloud Infrastructure Automation with Terraform (AWS)</h1>

<p align="center">
  <em>Next-Gen Cloud Infrastructure Automation | Built by Devesh Tyagi 🤖 | Powered by Terraform & AWS</em>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Terraform-v1.9.0-blueviolet?logo=terraform" />
  <img src="https://img.shields.io/badge/AWS-Cloud-orange?logo=amazonaws" />
  <img src="https://img.shields.io/badge/IaC-Infrastructure%20as%20Code-success?logo=githubactions" />
  <img src="https://img.shields.io/badge/DevOps-Automation-blue?logo=azuredevops" />
  <img src="https://img.shields.io/badge/Version%20Control-GitHub-black?logo=github" />
  <img src="https://img.shields.io/badge/License-MIT-green" />
</p>

---

## 📘 **Overview**
> **JOVAC (Job Oriented Value Added Course)** Multicloud infrastructure automation is an **AI-engineered Terraform project** that delivers *multi-cloud-ready infrastructure automation* on **AWS**.  
> It embodies the principles of **Infrastructure as Code (IaC)**, **idempotency**, and **scalability**, offering an enterprise-grade foundation for deploying and managing cloud workloads automatically.

This repository demonstrates:
- Modularized Terraform configurations 🧩  
- Automated EC2 provisioning with user data scripts ⚙️  
- Scalable load-balancing infrastructure 🌐  
- Version-controlled IaC deployment workflows via GitHub 🚀  

---

## ⚙️ **Tech Stack**

| Layer | Technology | Purpose |
|:------|:------------|:--------|
| ☁️ **Cloud Provider** | [AWS Cloud](https://aws.amazon.com/) | Infrastructure Hosting |
| 🧩 **IaC Tooling** | [Terraform v1.9.0+](https://www.terraform.io/) | Declarative Infrastructure Management |
| 🧠 **Automation** | Bash, PowerShell | Deployment & Bootstrap |
| 🔐 **Security** | AWS Security Groups, IAM Roles | Access Control |
| 🧾 **Version Control** | Git + GitHub | Source & State Management |
| 📦 **State Management** | Local / Remote (S3-ready) | Infrastructure State Persistence |
| 🧪 **Validation** | Terraform Validate + Plan | Pre-deploy checks |
| 💬 **Documentation** | Markdown + AI Enhanced Docs | Readable IaC Architecture |

---

## 🧭 **Project Architecture**

```plaintext
 ┌──────────────────────────────────────────┐
 │              Developer (You)             │
 └────────────────────┬─────────────────────┘
                      │
            ┌─────────▼──────────┐
            │   Terraform CLI    │
            └─────────┬──────────┘
                      │
             (Terraform Provider)
                      │
     ┌────────────────┴───────────────────┐
     │           AWS Cloud                │
     │────────────────────────────────────│
     │  • EC2 Instances                   │
     │  • Security Groups                 │
     │  • Load Balancer                   │
     │  • VPC, Subnets                    │
     │  • Key Pairs                       │
     └────────────────────────────────────┘
<img width="1024" height="1024" alt="Gemini_Generated_Image_8r9tgp8r9tgp8r9t" src="https://github.com/user-attachments/assets/14407aa1-9036-4ceb-99c0-223c406c321d" />
![AWS Terraform Infra](https://github.com/user-attachments/assets/ad550924-9712-489f-882c-11ce060d6e9b)
📁 Repository Structure
JOVAC_Terraform/
│
├── main.tf                  # Core Infrastructure definitions
├── provider.tf              # AWS provider configuration
├── variables.tf             # Input variables
├── userdata.sh              # Primary EC2 bootstrap script
├── userdata1.sh             # Alternative EC2 init script
├── terraform.tfstate        # Local Terraform state (ignored)
├── terraform.tfstate.backup # Backup state (ignored)
├── .terraform/              # Provider cache (ignored)
├── .gitignore               # Ignore Terraform & system files
└── README.md                # Documentation (AI-generated)
🚀 Deployment Steps
1️⃣ Initialize Terraform
terraform init

2️⃣ Validate the configuration
terraform validate

3️⃣ Preview changes before deploying
terraform plan

4️⃣ Deploy the infrastructure
terraform apply -auto-approve

5️⃣ Retrieve Load Balancer DNS (Output)
terraform output loadbalancerdns


✅ Example:

loadbalancerdns = "myalb-1432214074.us-east-1.elb.amazonaws.com"

6️⃣ Tear down infrastructure
terraform destroy -auto-approve

🧠 Best Practices Followed

📜 Modular Design: Easy to extend for multi-region or multi-cloud use.

🔁 Idempotent Deployments: Safe re-runs without state drift.

🔒 Secure Defaults: Minimal open ports, key-based SSH.

🧩 Reusable Code: Inputs/outputs standardized via variables.tf.

🧱 State Management: Configured for migration to AWS S3 + DynamoDB locks.

🧮 Automation-First: All steps scriptable and CI/CD ready.

🧰 DevOps Pipeline (Suggested Setup)
graph TD
A[Developer Commit] -->|Git Push| B[GitHub Actions CI/CD]
B --> C[Terraform Init & Validate]
C --> D[Terraform Plan]
D --> E[Manual Approval / Auto Trigger]
E --> F[Terraform Apply]
F --> G[AWS Infrastructure Live 🚀]


Can be integrated with GitHub Actions / Jenkins for full Continuous Deployment.

🌐 Future Roadmap
Milestone	Status
☁️ Multi-Cloud Expansion (Azure/GCP)	⏳ Planned
🧩 Terraform Modules Library	🔧 In Progress
🧠 AI-driven Infrastructure Recommendations	🚀 Experimental
🔄 S3 Backend Integration	✅ Completed
🔐 IAM Role Management	🧱 Pending
🧩 Tech Badges
<p align="center"> <img src="https://img.shields.io/badge/Terraform-IaC-blueviolet?style=for-the-badge&logo=terraform" /> <img src="https://img.shields.io/badge/AWS-Cloud-orange?style=for-the-badge&logo=amazonaws" /> <img src="https://img.shields.io/badge/Bash-Automation-black?style=for-the-badge&logo=gnubash" /> <img src="https://img.shields.io/badge/PowerShell-Scripting-0078D6?style=for-the-badge&logo=powershell" /> <img src="https://img.shields.io/badge/GitHub-Version%20Control-181717?style=for-the-badge&logo=github" /> <img src="https://img.shields.io/badge/AI-Generated%20Docs-00FFFF?style=for-the-badge&logo=openai" /> </p>
🧑‍💻 Author

👤 Devesh Tyagi
📍 Cloud & DevOps Engineer | Infrastructure Automation Specialist
💬 “Code your cloud. Automate your future.”
🔗 GitHub
 • LinkedIn

Crafted with ❤️ 

⚖️ License

Licensed under the MIT License — free for personal and commercial use.
Feel free to fork, improve, and build on this foundation.

🧩 Fun Fact

This entire README — architecture diagram, badges, and formatting — was generated and structured using AI-Driven Markdown Engineering, following OpenAI’s DevOps documentation style guidelines.
