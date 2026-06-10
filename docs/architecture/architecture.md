# CodeGen-AI Architecture

## LLD Diagram

![LLD](./lld-v1.png)

## Whimsical Source

https://whimsical.com/ridex4/codegen-ai-8praTpPd4nri433inB7k7W

---

## Overview

CodeGen-AI is an AI-powered full-stack application generation platform inspired by Lovable.

The system generates, stores, retrieves, and executes code using LLMs, RAG, and isolated execution environments.

---

## Core Components

### API Gateway

Responsibilities:

- Accept user prompts
- Authentication
- Request routing
- SSE streaming

### Intelligent Service

Responsibilities:

- Prompt orchestration
- Tool calling
- Context management
- LLM communication

### Workspace Service

Responsibilities:

- Project metadata
- Session history
- File management

### RAG Layer

Responsibilities:

- Embedding generation
- Similarity search
- Context retrieval

### Execution Service

Responsibilities:

- Isolated code execution
- Preview generation
- Runtime management

### Storage

- S3 for generated artifacts
- Vector DB for embeddings

### Messaging

- Kafka for asynchronous processing
- Event-driven communication

---

## Future Improvements

- Multi-agent workflows
- OpenTelemetry tracing
- Kubernetes autoscaling
- Multi-tenant architecture