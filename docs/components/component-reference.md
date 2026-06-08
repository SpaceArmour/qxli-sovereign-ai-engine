# QXLI Component Reference

## Overview

QXLI Sovereign AI Engine is built on a collection of proven open-source technologies that together provide a complete sovereign AI platform.

Rather than relying on a single monolithic system, QXLI combines specialized components for user interaction, language model execution, workflow automation, retrieval-augmented generation (RAG), observability, identity management, and infrastructure services.

Each component fulfills a dedicated role while contributing to a unified private AI environment.

---

## User Experience Layer

### Open WebUI

Open WebUI provides the primary user-facing interface for QXLI.

It delivers a self-hosted AI experience that allows users to interact with private language models, access organizational knowledge, and engage with AI-powered workflows through a governed environment.

**Role within QXLI:**

* Primary user interface
* Self-hosted AI interaction
* Access point for assistants and knowledge systems

---

## AI Runtime Layer

### vLLM

vLLM serves as the core language model inference engine within QXLI.

It enables organizations to run private large language models on infrastructure they control while avoiding dependency on external AI APIs.

**Role within QXLI:**

* Private model execution
* Local inference runtime
* Foundation for AI-generated responses

---

## AI Gateway Layer (Optional)

### LiteLLM

LiteLLM provides an optional gateway layer that can centralize model access, routing, policy controls, and usage management.

It offers a unified interface for managing multiple model endpoints.

**Role within QXLI:**

* Model routing
* Access control layer
* Unified AI gateway

---

## Agent & Orchestration Layer

### LangChain

LangChain provides a framework for developing AI-powered applications and connecting language models to external tools and services.

**Role within QXLI:**

* Application framework
* AI workflow integration
* Tool and service connectivity

---

## Workflow Automation Layer

### n8n

n8n connects AI capabilities to operational business workflows.

It enables automation across applications, databases, notifications, approval processes, and enterprise systems.

**Role within QXLI:**

* Workflow automation
* System integration
* Business process connectivity

---

## Data & RAG Layer

### PostgreSQL

PostgreSQL serves as the primary structured data platform within QXLI.

It stores application data, metadata, and operational information required by the platform.

**Role within QXLI:**

* Structured data storage
* Metadata management
* Persistent platform data

---

### pgvector

pgvector extends PostgreSQL with vector search capabilities.

It enables semantic retrieval, embedding storage, and retrieval-augmented generation (RAG) workflows.

**Role within QXLI:**

* Vector storage
* Semantic search
* Knowledge retrieval

---

## Governance & Observability Layer

### Langfuse

Langfuse provides observability and operational visibility across AI workloads.

It supports tracing, monitoring, evaluation, and debugging of language model interactions.

**Role within QXLI:**

* Observability
* Prompt tracing
* Operational monitoring
* Governance support

---

## Identity & Access Layer

### Keycloak

Keycloak provides enterprise identity and access management capabilities.

It supports authentication, authorization, role-based access control, and single sign-on integration.

**Role within QXLI:**

* Identity management
* Access control
* Enterprise authentication

---

## Infrastructure Layer

### NGINX

NGINX provides ingress, routing, and traffic management capabilities for the platform.

It serves as a gateway between users and internal services.

**Role within QXLI:**

* Traffic routing
* HTTPS and TLS support
* Ingress management

---

### NVIDIA AI Blueprints

NVIDIA AI Blueprints provide reference architectures and deployment guidance that can support high-performance AI environments.

These resources help organizations accelerate the adoption of private AI capabilities.

**Role within QXLI:**

* Reference architectures
* AI acceleration guidance
* Enterprise AI enablement

---

## Component Relationships

The QXLI Sovereign AI Engine combines these components into a unified platform architecture.

At a high level:

1. Users interact through Open WebUI.
2. Requests may be routed through LiteLLM when gateway capabilities are required.
3. vLLM executes private language models.
4. LangChain supports AI workflows and agent behavior.
5. PostgreSQL and pgvector provide structured and semantic knowledge access.
6. n8n connects AI outputs to operational business processes.
7. Langfuse provides observability and governance visibility.
8. Keycloak manages identity and access control.
9. NGINX provides secure ingress and routing.

Together, these components create a modular sovereign AI platform that remains under organizational control.

---

## Summary

QXLI Sovereign AI Engine is built upon a carefully selected collection of open-source technologies that each provide a specific capability within the platform.

By combining user experience, AI runtime, orchestration, automation, data management, governance, security, and infrastructure services, QXLI delivers a unified sovereign AI environment designed for enterprise deployment and long-term operational control.
