# Nexus-
Nexus AI
NX1-AI-CORE-001

NEXUS Independent AI Core

Project ID: NX1-AI-CORE-001
Version: 1.0.0-DRAFT
Status: Development
Architecture: Hybrid AI Core
Database: PostgreSQL
Primary AI Provider: Hugging Face
Budget Policy: 0 THB
Repository: https://github.com/aesebu/Nexus-
Hugging Face: https://huggingface.co/Aesebu/NX1-AI-CORE-001

---

1. Project Overview

NX1-AI-CORE-001 is an independent AI core project within the NEXUS ecosystem.

The objective is to develop a modular AI foundation that supports model registration, provider integration, intelligent routing, evaluation, auditing, and future autonomous capabilities.

The system is designed to support multiple AI model providers through a unified architecture.

Core Objectives

- Independent and modular AI architecture.
- Centralized AI Model Registry.
- Multi-provider integration.
- PostgreSQL-based data management.
- Cost-aware AI routing.
- Thai-language AI evaluation.
- Auditable inference operations.
- Future support for autonomous learning and agent systems.

2. System Architecture

NX1 AI CORE
│
├── Core Foundation
│   ├── Configuration
│   ├── Core Interfaces
│   └── Error Handling
│
├── Model Management
│   ├── Model Registry
│   ├── Model Metadata
│   └── Model Ranking
│
├── Provider Layer
│   ├── Hugging Face Adapter
│   ├── Provider Interface
│   └── Future Provider Adapters
│
├── AI Routing Engine
│   ├── Model Selection
│   ├── Cost Eligibility Gate
│   └── Request Routing
│
├── Evaluation Engine
│   ├── Thai Benchmark
│   ├── Human Evaluation
│   └── Performance Scoring
│
├── Audit System
│   ├── Request Logs
│   └── Cost Records
│
└── PostgreSQL Database

3. Technology Stack

Component| Technology
Backend| Python
Database| PostgreSQL
AI Model Source| Hugging Face
Database Adapter| Psycopg 3
Model Integration| Hugging Face Hub
Testing| Pytest
Deployment| Docker
Source Control| GitHub

4. Development Phases

Phase| Description
01.1| Core Foundation
01.2| Provider Abstraction
01.3| PostgreSQL Model Registry & Audit
01.4| Hugging Face Adapter
01.5| Metadata Validation & Cost Gate
01.6| Thai Benchmark & Human Evaluation
01.7| Runtime and Cost Safety
01.8| Application Runtime Foundation
01.9| Release Preflight
02.0| Source Integration
02.1| Compatibility and Integration Tests

Important: Phase 01.1–01.6 source reconstruction is a new implementation based on available project specifications. It must not be represented as recovered historical source code.

5. Database

The project uses PostgreSQL for persistent model and inference management.

Core data entities:

- "nx1_model_providers"
- "nx1_models"
- "nx1_inference_requests"

Database changes must use version-controlled migrations.

Migration requirements:

- Prepared migration.
- Schema validation.
- Rollback plan.
- Automated tests.
- Explicit approval before production changes.

Never apply an unreviewed migration to the main database.

6. AI Provider Integration

Hugging Face

Hugging Face is the primary model source for this project.

Responsibilities:

- Model metadata discovery.
- Model repository inspection.
- License validation.
- Model capability classification.
- Inference adapter integration.

Repository:

https://huggingface.co/Aesebu/NX1-AI-CORE-001

Model inference must remain disabled until cost eligibility and operational safety have been verified.

7. Zero-Cost Policy

The project currently operates under a 0 THB budget.

Mandatory rules:

1. No paid API requests without explicit approval.
2. Unknown pricing must be blocked.
3. Verify official pricing and free-tier quota before inference.
4. No automatic paid endpoint provisioning.
5. No automatic provider fallback that can generate charges.
6. Record blocked requests in the audit system.
7. Keep live inference disabled by default.

A free-tier label alone is not sufficient evidence that an inference request is cost-free.

8. Thai AI Evaluation

The evaluation framework includes:

- Thai language comprehension.
- Thai language fluency.
- Instruction following.
- Reasoning.
- Mathematical accuracy.
- Factual accuracy.
- Hallucination risk.
- Safety.
- Construction-domain knowledge.

The initial benchmark contains 20 test cases.

Reference answers are evaluation guidance and must undergo human review before being treated as certified evaluation data.

9. Installation

Clone the repository:

git clone https://github.com/aesebu/Nexus-.git
cd Nexus-

Create a Python environment:

python -m venv .venv

Activate the environment:

# Linux / macOS
source .venv/bin/activate

# Windows
.venv\Scripts\activate

Install dependencies:

pip install -e ".[test]"

Optional PostgreSQL dependencies:

pip install -e ".[postgres]"

Optional Hugging Face dependencies:

pip install -e ".[huggingface]"

Run tests:

pytest

10. Environment Configuration

Example ".env.example":

DATABASE_URL=
HF_TOKEN=

NX1_BUDGET_THB=0
NX1_ALLOW_LIVE_INFERENCE=false
NX1_REQUEST_TIMEOUT=10

Never commit real secrets or credentials.

11. Security

- Keep tokens in environment secrets.
- Never expose database credentials.
- Use PostgreSQL SSL connections.
- Validate model metadata and licenses.
- Block unknown inference costs.
- Maintain inference audit records.
- Require explicit authorization for production changes.

12. Repository Structure

NX1-AI-CORE-001/
│
├── README.md
├── pyproject.toml
├── .env.example
├── Dockerfile
│
├── src/
│   └── nx1_core/
│       ├── config.py
│       ├── models.py
│       ├── interfaces.py
│       ├── registry.py
│       ├── postgres.py
│       ├── huggingface.py
│       ├── cost_gate.py
│       ├── router.py
│       ├── audit.py
│       ├── validators.py
│       ├── benchmark.py
│       ├── ranking.py
│       └── evaluation.py
│
├── migrations/
│
├── tests/
│
├── docs/
│
└── scripts/

This structure is the target layout; actual file availability must be verified before release.

13. Development Status

Item| Status
Project architecture| Draft specification
PostgreSQL foundation| Previously installed tables
Hugging Face integration| Development
Cost Gate| Fail-closed design
Thai benchmark| 20-case specification
Phase 01.1–01.6 reconstruction| Pending source package delivery
GitHub upload| Not verified
Docker deployment| Not verified
Live inference| Disabled

14. License

The project license has not yet been finalized.

Do not assume that the licenses of third-party models are identical to the license of this repository.

---

NEXUS AI — NX1-AI-CORE-001

Independent AI Core Development Project

Document classification: DRAFT
Last updated: 2026-11-11
