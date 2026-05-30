\# CO 533: Advanced Computational Intelligence — Laboratory 02



This repository contains my implementation and verification data for Laboratory 02, focusing on the deployment of \*\*Agentic Workflow Patterns\*\*. The core architecture utilizes an open-source local LLM runtime engine (`qwen3:8b` executed via Ollama) integrated with Python-based orchestration layers.



\## Technical Objectives \& Architecture

The goal of this laboratory is to move beyond stateless, single-turn LLM prompts and implement deterministic, multi-step agentic systems:

1\. \*\*Prompt Chaining with Error Recovery:\*\* Programmatic evaluation loops that catch structural parsing errors and trigger automated retries.

2\. \*\*Dynamic Semantic Routing:\*\* Conditional triage systems that classify unstructured user queries into specialized downstream execution domains.

3\. \*\*Parallel Execution Layer:\*\* Multi-threaded processing using Python concurrency pools to perform synchronous content generation and safety evaluations.



\## Local Environment Configuration

To replicate these execution results, the environment must be configured as follows:



1\. \*\*Local Runtime:\*\* Ollama must be active and serving weights locally.

2\. \*\*Model Dependency:\*\* Pull the workspace baseline model:

&#x20;  ```bash

&#x20;  ollama pull qwen3:8b

