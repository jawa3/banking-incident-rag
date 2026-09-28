# Banking Incident RAG

A Retrieval-Augmented Generation (RAG) application for analyzing banking production incidents.

The system uses:

- Python
- LangChain
- LangGraph
- FAISS
- Sentence Transformers
- OpenAI / Azure OpenAI
- FastAPI
- Docker
- Kubernetes
- GitHub Actions

## Architecture

Banking Documents
        |
        v
Document Loader
        |
        v
Chunking
        |
        v
Embeddings
        |
        v
FAISS Vector Store
        |
        v
Retriever
        |
        v
RAG Generator
        |
        v
LangGraph Incident Analyzer
        |
        v
FastAPI
        |
        v
Docker / Kubernetes

## Use Case

Example incident:

"Payment transactions are failing in the production environment."

The system retrieves:

- Payment policies
- Previous incident RCA documents
- AWS runbooks
- EKS troubleshooting documentation

Then it generates:

- Incident summary
- Possible root cause
- Relevant evidence
- Recommended troubleshooting steps
- Runbook
- Suggested remediation

## Project Structure

See the project directory for ingestion, vectorstore, RAG, LangGraph,
API, testing and deployment components.

## Run

Install dependencies:

```bash
pip install -r requirements.txt
