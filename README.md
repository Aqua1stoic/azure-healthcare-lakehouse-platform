# 🚀 Modern Data Engineering Portfolio – Azure, Databricks, IoT, Healthcare, AI, Streaming

A curated collection of production-grade data engineering projects, reference architectures, Terraform deployments, streaming pipelines, notebooks, and AI-ready workflows.
This repository is designed as a real-world engineering portfolio showcasing mastery across Azure, Databricks, IoT, Event Hubs, Delta Lake, ML pipelines, vector databases, and enterprise security (RBAC + Key Vault).

This repo is intentionally structured like an internal platform engineering codebase you’d find at senior-level roles in healthcare, fintech, industrial IoT, AI startups, and cloud-native enterprises.

## 🎯 Purpose

This repository serves as a central hub for:

End-to-end data engineering projects

Azure cloud infrastructure (Terraform)

Real-time streaming pipelines (IoT Hub → Event Hubs → Databricks)

Batch + streaming Lakehouse patterns (Bronze → Silver → Gold)

AI/ML feature stores & vector database integrations

FHIR/EHR/healthcare data ingestion pipelines

Airflow orchestration

API ingestion connectors

Analytics-ready semantic layers (Power BI / Superset)

It demonstrates not just “tutorial skills,” but the real systems and patterns used by senior data engineers in the industry.

## 🏛️ Architecture & Philosophy

This repo follows a consistent engineering philosophy:

✔ Infrastructure as Code first

Everything deployable is defined in Terraform modules.

✔ Modular, reusable ingestion layers

API → IoT → FHIR → Raw
Each ingestion style has its own subfolder and utils.

✔ Delta Lake Medallion Architecture

All processing aligns to Bronze → Silver → Gold curation patterns.

✔ Security by default

RBAC, Key Vault, no secrets in code, least-privilege access.

✔ AI-ready tables and embeddings

Every project either produces ML feature tables, vector embeddings, or predictive features.

✔ End-to-end lifecycle

Ingestion → Transformation → Curation → ML → BI.

## 📂 Repository Structure
```data-engineering-projects/
│
├── 00-foundations/                # Shared utilities, schemas, helpers
│
├── 01-infrastructure/             # Terraform, Bicep, CI/CD workflows
│   ├── terraform/
│   └── ci-cd/
│
├── 02-ingestion/                  # API, IoT, FHIR, streaming, Airflow
│   ├── api-connectors/
│   ├── fhir-ingestion/
│   ├── iot-simulators/
│   ├── airbyte-connectors/
│   └── airflow-dags/
│
├── 03-processing/                 # Databricks notebooks, Spark jobs
│   ├── databricks/
│   ├── streaming-jobs/
│   └── pyspark-jobs/
│
├── 04-lakehouse/                  # Delta tables, medallion logic
│   ├── bronze/
│   ├── silver/
│   └── gold/
│
├── 05-ai-ml/                      # Feature store, embeddings, MLflow
│   ├── vector-db/
│   ├── feature-engineering/
│   └── models/
│
├── 06-bi-and-analytics/           # Power BI, Superset, SQL semantic layer
│   ├── powerbi/
│   └── superset/
│
├── docs/                          # Architecture diagrams, explanations
│   ├── architecture-diagrams/
│   ├── sequence-diagrams/
│   └── readme-assets/
│
├── scripts/                       # deployment, automation, local tools
│
└── README.md
```

This structure mirrors enterprise data engineering teams:
modular, scalable, multi-project, and multi-pipeline.

## 🌐 Highlighted Projects Inside This Repo

### 🔥 Healthcare IoT Real-Time Lakehouse (Azure + Databricks)

IoT Hub → Event Hubs → Databricks Streaming

Delta Medallion

Patient-level risk scoring

Vector embeddings for clinical notes

Terraform provisioning

Enterprise RBAC + Key Vault

### ⚙️ Terraform Azure Data Platform

Full infra-as-code deployment

Databricks workspace

ADLS Gen2

Key Vault

Event Hubs

Role assignments

### ☁️ API + FHIR Ingestion Framework

Production-ready API ingestion templates

FHIR Observation/Encounter mapping

Schema registry for healthcare payloads

### 🌀 Airflow DAG Collections

ELT automation

Triggering databricks jobs

Backfill orchestration

### 📊 BI & Analytics Layer

Gold views

Power BI templates

Semantic modelling patterns


## 🛡️ Security & Compliance Standards Followed

This repo follows HIPAA/SOC2-aligned practices:

✔ RBAC least privilege
✔ Zero secrets in code (Key Vault + .env.example)
✔ Managed Identity for Databricks → Storage/Event Hubs
✔ Private endpoints (recommended)
✔ Versioned, auditable data (Delta Lake)
✔ Terraform state security

These patterns are used in real medical, fintech, and IoT deployments.

## 🚀 Getting Started
1. Clone the repo
git clone https://github.com/Aqua1stoic/azure-healthcare-lakehouse-platform.git

2. Navigate into the repo
cd azure-healthcare-lakehouse-platform

3. Install prerequisites

You should have:

Azure CLI

Terraform

Python 3.10+

Databricks CLI

Docker (optional)

Power BI Desktop (optional)


## 🔧 Local Environment Setup
Install python dependencies:
pip install -r requirements.txt

Setup environment file:
cp .env.example .env

Login to Azure:
az login

Setup databricks:
databricks configure --aad-token

## 🧰 Tooling Standards
The repo follows the following tooling approaches:

Code Quality

Black (formatting)

Ruff (linting)

Pre-commit hooks

Git Standards

Conventional commits

Feature-branch workflow

Protected main branch

## 🎓 Skills Demonstrated

By using this repo, you show proficiency in:

### Cloud

Azure IoT Hub
Event Hubs
ADLS Gen2
Databricks
Key Vault
Azure Functions
Azure Batch

### Data Engineering

Spark / PySpark
Delta Lake
Streaming & Batch pipelines
Medallion Architecture
Orchestration (Airflow)
Schema evolution
CDC patterns

### Infra & Security

Terraform
RBAC
IAM
Private networking
Key Vault secrets management

### AI/ML

MLflow
Feature engineering
Vector DB (pgvector / Databricks Vector Search)
Embedding pipelines

### Analytics

Databricks SQL
Power BI
Materialized views
Semantic layers

## 🧭 Roadmap
✔ IoT Healthcare Lakehouse

✔ Terraform full platform buildout

✔ API ingestion templates

✔ Vector DB integration

⬜ Add DLT (Delta Live Tables) pipelines

⬜ Add CI/CD workflows (GitHub Actions)

⬜ Add Snowflake ingestion variant

⬜ Add dbt model folder

⬜ Build a microservice ingestion API in FastAPI

You can extend this repo indefinitely.

## 📫 Contact

For collaboration, questions, or advanced architecture design:
Email: aquaintuition@gmail.com

LinkedIn: www.linkedin.com/in/samuel-ntui-akwa

🏁 Final Note

This repository isn’t a set of “projects.”
This is a full data engineering platform and a long-term technical portfolio I will keep expanding.

👉 “I design and build real data systems, not toy notebooks.”
