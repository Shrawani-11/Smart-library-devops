# SMART LIBRARY MANAGEMENT PLATFORM
## DevOps Project Documentation Report

**Project Title:** Smart Library Management Platform  
**Project Domain:** DevOps and Cloud Computing  
**Cloud Platform:** Amazon Web Services (AWS)  
**Tools and Technologies:** Terraform, Ansible, Docker, Nginx, Git, GitHub, Ubuntu Linux

---

# 1. Project Overview

The Smart Library Management Platform is a lightweight web application deployed on an Amazon Web Services (AWS) EC2 instance. This project demonstrates the use of DevOps tools to automate cloud infrastructure provisioning, server configuration, and web application deployment.

Terraform is used to provision the required AWS infrastructure, including a Virtual Private Cloud (VPC), subnet, internet gateway, security group, EC2 instance, and S3 bucket. Ansible automates the configuration of the target server and the deployment process. Docker is used to containerize the application, while Nginx serves the web page.

Git and GitHub are used to maintain and manage the project's source code and configuration files.

# 2. Project Objectives

The main objectives of this project are:

1. To provision AWS infrastructure using Terraform.
2. To create and configure a VPC, public subnet, internet gateway, security group, EC2 instance, and S3 bucket.
3. To install and configure Docker on the target EC2 instance.
4. To automate server configuration and application deployment using Ansible.
5. To deploy and host the web application using Docker and Nginx.
6. To verify application accessibility through HTTP.
7. To maintain the project source code using Git and GitHub.
8. To apply basic security practices while managing cloud resources and project files.

# 3. Technologies Used

The following tools and technologies are used in this project.

| Technology | Purpose |
|---|---|
| Amazon Web Services (AWS) | Cloud infrastructure and hosting |
| Amazon EC2 | Virtual server for application deployment |
| Amazon S3 | Object storage and backup bucket |
| Terraform | Infrastructure provisioning using Infrastructure as Code |
| Ansible | Server configuration and deployment automation |
| Docker | Application containerization |
| Nginx | Web server for serving the application |
| Ubuntu Linux | Operating system for the EC2 instance |
| Git | Version control |
| GitHub | Remote source code repository |

**[Insert Screenshot 1: Software versions and environment details]**

# 4. Project Structure

The project is organized into separate directories to manage the application, infrastructure, deployment automation, and documentation.

```text
smart-library-devops/
├── app/
│   ├── index.html
│   └── Dockerfile
├── ansible/
│   ├── deploy-library.yml
│   └── inventory.ini.example
├── terraform/
│   ├── main.tf
│   └── .terraform.lock.hcl
├── docs/
│   └── screenshots/
├── .gitignore
└── README.md
```

**Description of directories and files:**

- **app/** – Contains the application HTML file and Dockerfile.
- **ansible/** – Contains the Ansible playbook and an example inventory file.
- **terraform/** – Contains Terraform configuration files for AWS infrastructure.
- **docs/screenshots/** – Stores screenshots showing project implementation and results.
- **.gitignore** – Specifies files and directories that should not be tracked by Git.
- **README.md** – Provides project information, setup instructions, and usage details.

**[Insert Screenshot 2: GitHub repository showing the project structure]**

# 5. Infrastructure Provisioning Using Terraform

Terraform is an Infrastructure as Code (IaC) tool used to define and provision cloud resources through configuration files. In this project, Terraform is used to create the AWS infrastructure required to host the Smart Library Management Platform.

The infrastructure includes the following resources:

1. **Virtual Private Cloud (VPC):** Provides an isolated network environment.
2. **Public Subnet:** Hosts the EC2 instance and allows public connectivity when correctly configured.
3. **Internet Gateway:** Enables communication between the VPC and the internet.
4. **Route Table:** Directs eligible outbound traffic through the internet gateway.
5. **Security Group:** Controls inbound and outbound network traffic.
6. **EC2 Instance:** Provides the virtual server for application deployment.
7. **S
