# 💰 infra-cost-analysis

Simulated cost breakdowns of AWS infrastructure designs, built with a cost-conscious mindset and an emphasis on aligning engineering decisions with business and budgetary objectives.

## 📌 Overview

This repository analyzes the cost implications of various AWS architectural patterns. Each scenario explores how technical design choices—like compute type, storage tiering, redundancy, and data transfer—impact your monthly AWS bill.

The goal is to bridge the gap between engineering excellence and fiscal responsibility, empowering developers and architects to make decisions that are both scalable and cost-effective.

💡 Special focus is given to S3 storage pricing, including:
- Storage class selection (Standard, IA, Glacier)
- Data retrieval and lifecycle transitions
- Inter-region and cross-AZ transfer fees

## 🔎 What’s Included

Each scenario folder includes:
- 🖼️ `design-diagram.png`: Architecture diagram
- 📊 `cost-breakdown.md`: Annotated cost breakdown using AWS Pricing Calculator
- 📝 `summary.txt`: Business and engineering tradeoff notes

Scenarios involving S3 usage also highlight:
- 🔐 Storage class used (Standard, IA, One Zone, Glacier, etc.)
- ♻️ Lifecycle rules for auto-tiering
- 🚚 Data egress costs (to other services, regions, or internet)

## 💼 Use Cases

- ✅ Certification prep (AWS SAA-C03, CCP)
- ✅ DevOps & cloud engineering interviews
- ✅ Internal cost estimation and architecture review
- ✅ Devs shifting from code-first to cost-aware mindset

## 📚 Learning Goals

- Understand the cost of core AWS services in real-world deployments
- Compare compute vs serverless tradeoffs
- Evaluate the total cost of S3 storage, retrieval, and transfer
- Balance performance, reliability, and cost in design
- Translate architectural decisions into financial impact

## ⚙️ Tools & References

- AWS Pricing Calculator
- AWS S3 Pricing Docs (https://aws.amazon.com/s3/pricing/)
- Cloud architecture diagrams
- Excel + markdown modeling
- [AWS Well-Architected Framework](https://aws.amazon.com/architecture/well-architected/)

## 🚀 Roadmap

- Add ECS + Fargate vs EC2 cost comparison
- Add Spot Instance usage simulations
- Add S3 Glacier tier analysis and archival lifecycle tests
- Automate price generation via `boto3` or pricing APIs
- Add Azure and GCP equivalents (multi-cloud pricing)
