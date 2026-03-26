# Hi, I'm Raseef Azeez

### Cloud Infrastructure Engineer → DevOps → Cloud Architecture

Cloud Engineer with 5+ years of AWS experience, focused on building automated, scalable, and resilient cloud-native systems using Terraform, Kubernetes, and modern CI/CD practices.

I enjoy working on systems that don’t just run — but **recover, scale, and adapt**.

I believe in **architecting simplicity in the cloud** — breaking down complex systems by asking one **“why”** at a time, and designing solutions that are easy to operate, reason about, and evolve.

---

## 🌐 Connect With Me

[![LinkedIn](https://img.shields.io/badge/LinkedIn-blue?style=for-the-badge\&logo=linkedin)](https://www.linkedin.com/in/raseef-azeez)
[![Portfolio](https://img.shields.io/badge/Portfolio-Website-black?style=for-the-badge\&logo=google-chrome)](https://d3svccsjj104ji.cloudfront.net)

---

## Architecting Simplicity in the Cloud

My approach to cloud engineering is centered around:

* **Clarity over complexity** — systems should be easy to understand and debug
* **Automation by default** — reduce manual effort through repeatable workflows
* **Resilience by design** — build systems that fail gracefully and recover quickly
* **Progressive evolution** — start simple, then scale and optimize

---

## 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=RaseefAzeez&show_icons=true&theme=radical&hide_border=true" height="150"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=RaseefAzeez&layout=compact&theme=radical&hide_border=true" height="150"/>
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com?user=RaseefAzeez&theme=radical&hide_border=true"/>
</p>

---

## 🛠 Tech Stack

### ☁️ Cloud & DevOps

![AWS](https://img.shields.io/badge/AWS-orange?style=for-the-badge\&logo=amazon-aws)
![Terraform](https://img.shields.io/badge/Terraform-purple?style=for-the-badge\&logo=terraform)
![Kubernetes](https://img.shields.io/badge/Kubernetes-blue?style=for-the-badge\&logo=kubernetes)
![Docker](https://img.shields.io/badge/Docker-blue?style=for-the-badge\&logo=docker)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-black?style=for-the-badge\&logo=github-actions)

### ⚙️ Serverless & Backend

![AWS Lambda](https://img.shields.io/badge/Lambda-orange?style=for-the-badge\&logo=aws-lambda)
![API Gateway](https://img.shields.io/badge/API_Gateway-orange?style=for-the-badge\&logo=amazon-api-gateway)
![DynamoDB](https://img.shields.io/badge/DynamoDB-blue?style=for-the-badge\&logo=amazon-dynamodb)

### 📊 Observability

![CloudWatch](https://img.shields.io/badge/CloudWatch-orange?style=for-the-badge\&logo=amazon-cloudwatch)
![Prometheus](https://img.shields.io/badge/Prometheus-orange?style=for-the-badge\&logo=prometheus)
![Grafana](https://img.shields.io/badge/Grafana-orange?style=for-the-badge\&logo=grafana)

---

## 🎖 Certifications

<a href="https://www.credly.com/badges/bb09b07e-814c-436f-b136-25ad12022d3d" target="_blank">
  <img src="https://img.shields.io/badge/AWS_Certified-Solutions_Architect_Associate-orange?style=for-the-badge&logo=amazon-aws&logoColor=white" alt="AWS Certified Solutions Architect – Associate (SAA-C03)">
</a>

---

## Flagship System: RaaS (Reboot as a Service)

RaaS is a self-service platform designed to **reduce operational overhead by enabling users to independently troubleshoot and recover access to their EC2 instances or workspaces**.

Instead of relying on support teams for routine access issues, users can:

* Reboot their assigned instances
* Check instance status
* Recover access without raising tickets

---

### 🎯 Why RaaS?

In real-world environments, a large portion of support tickets are generated due to:

* Users unable to SSH / RDP into instances
* Workspace access issues
* Delays in support response

RaaS shifts this model:

```text
Support-driven operations → Self-service automation
```

📉 Result:
**Reduces support ticket volume by ~20–25% (realistic impact)**

---

### 🏗 Architecture

![RaaS Architecture](./architecture.png)

---

### ⚙️ How It Works

```text
User → Cognito Login → S3 (Frontend via CloudFront)
         ↓
     API Gateway (JWT Authorizer)
         ↓
        Lambda
         ↓
   EC2 Actions (Reboot / Status / Access Check)
```

---

### 🔐 Identity & Access Design

#### Authentication

* **Amazon Cognito (JWT-based authentication)**

#### Identity Management

* **IAM Identity Center (SSO)** with AWS Organizations
* Centralized user and group control

#### Authorization (ABAC)

* Attribute-Based Access Control using **EC2 instance tags**
* Users can only access instances mapped to their group

```text
User Group → Tag Match → Allowed Instance Access
```

✔ No hardcoded permissions
✔ Scalable multi-user model
✔ Clean separation of access

---

### Design Principles (Simplicity in Practice)

* **No database required** → Stateless, lightweight design
* **Minimal services** → S3 + API Gateway + Lambda + Cognito
* **Policy-driven access** → ABAC over static roles
* **Self-service first** → Reduce operational dependency

---

### ⚡ Key Highlights

* **Frontend:** S3 + CloudFront
* **Backend:** API Gateway + Lambda
* **Auth:** Cognito JWT
* **Access Control:** IAM Identity Center + ABAC
* **Automation:** Terraform + GitHub Actions (OIDC, no static credentials)

---

### 📈 Impact

* 🔻 Reduced support tickets by **20–25%**
* ⚡ Faster issue resolution
* 🔐 Improved security model
* 🧩 Simplified architecture

---

### 🔄 Evolution (RaaS v2 — In Progress)

```text
Serverless → Kubernetes (Containerized Platform)
```

Goal:

* Better observability
* More control
* Platform scalability

---

## 📂 Other Projects

### 🔹 Cloud Portfolio Platform

* Serverless architecture using S3, CloudFront, Lambda, and DynamoDB
* 🔗 [View Portfolio](https://d3svccsjj104ji.cloudfront.net)
* 📝 [Read the Build Story](https://raseefazeez.hashnode.dev/how-i-built-my-cloud-portfolio-using-aws-and-github-actions)

---

## 📈 Current Focus (RaaS v2)

* Containerizing **RaaS → Kubernetes (KIND / k3s)**
* Building **CI/CD pipelines (Docker → K8s deployment)**
* Deepening **Observability (Prometheus & Grafana)**
* Exploring **multi-cloud patterns**

---

### 🔹 Kubernetes & CI/CD Lab (RaaS v2)

* **Kubernetes:** Deployments, Ingress, ConfigMaps (In Progress)
* **CI/CD:** Multi-stage GitHub Actions (Build → Push → Deploy)
* **IaC:** Modular Terraform (VPC, IAM, reusable modules)

---

## Beyond Tech

I believe good engineers don’t just build systems — they **reduce complexity, anticipate failure, and design for clarity**.

---

## Contribution Activity

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=RaseefAzeez&theme=github-dark&hide_border=true"/>
</p>

