# Syllabus

Every module in the hub, by course and track. Times are the estimated study time per module.

## Production RAG, Agents and LLM Engineering

40 modules, about 38 hours.


**Foundations**: The mental model and the machinery under it

1. What RAG is, and the naive pipeline (40 min)
2. Embeddings and similarity, properly (60 min)
3. How LLM inference works, for engineers (50 min)
4. Vector search internals: brute force, HNSW, IVF, PQ (70 min)
5. BM25 and sparse retrieval (45 min)

**RAG in production**: From naive pipeline to something you can operate

6. Production RAG architecture (60 min)
7. Parsing, where quality is won or lost (55 min)
8. Chunking, contextual retrieval and small-to-big (65 min)
9. Hybrid search, fusion and query rewriting (50 min)
10. Reranking, diversity and context assembly (55 min)
11. Debugging a RAG system that gives wrong answers (60 min)
12. Measuring RAG quality (65 min)
13. Access control in RAG (60 min)
14. Freshness, deletes and reindexing (55 min)
15. Long context versus RAG (40 min)
16. Reducing hallucination (55 min)
17. Latency and cost in the query path (50 min)
18. Fine-tuning versus RAG (50 min)
19. Capstone: RAG for a large enterprise knowledge base (75 min)

**Agents**: Loops, tools, budgets and the ways they fail

20. Tool calling and the agent loop (45 min)
21. Agent or workflow? (45 min)
22. Building a production agent harness (65 min)
23. Managing context over long agent runs (55 min)
24. Designing tools, the execution wrapper and MCP (60 min)
25. Evaluating agents (50 min)
26. Where agents fail in production (40 min)
27. When multi-agent actually helps (35 min)
28. Human approval and graduated autonomy (45 min)

**LLM production engineering**: Reliability, security, cost, deploys, evals

29. Reliable structured output (60 min)
30. Prompts as code (50 min)
31. Resilience: outages, rate limits and degradation (65 min)
32. Cost control (50 min)
33. Prompt injection and the security architecture (70 min)
34. Deploying changes safely (55 min)
35. Observability: tracing, metrics and the feedback loop (55 min)
36. Building an evaluation practice from scratch (70 min)
37. Self-hosting versus APIs, and how serving works (70 min)
38. Choosing a model (45 min)

**Interview performance**: Design rounds, stories, and the final drill

39. System design rounds (90 min)
40. Experience stories, your questions, the cram sheet and the final drill (75 min)

## Fine-tuning and Model Adaptation

40 modules, about 37 hours.


**Deciding and preparing**: Whether to tune at all, and the data and evals that decide the outcome

1. When to fine-tune, and when not to (50 min)
2. The adaptation landscape (45 min)
3. Data is the product (65 min)
4. Formatting, templates and loss masking (50 min)
5. Build the evaluation first (55 min)

**Methods**: Full fine-tuning, LoRA, QLoRA and the rest of the adapter family

6. Full fine-tuning mechanics (55 min)
7. LoRA (70 min)
8. QLoRA and quantised training (60 min)
9. The rest of the adapter family (50 min)
10. Serving adapters (50 min)
11. Continued pretraining and domain adaptation (55 min)
12. Catastrophic forgetting (50 min)

**Training craft**: Hyperparameters, memory, stability and reading the curves

13. Hyperparameters that matter (55 min)
14. The training loop in practice (55 min)
15. Memory, speed and multi-GPU (55 min)
16. Stability and debugging a failing run (55 min)
17. Reading curves, overfitting and memorisation (50 min)
18. Multi-task training and data mixing (50 min)

**Alignment and preferences**: Reward models, RLHF, DPO and reasoning training

19. Preference data (55 min)
20. Reward models (55 min)
21. RLHF with PPO and GRPO (65 min)
22. DPO and the direct alignment family (65 min)
23. Reasoning training with verifiable rewards (60 min)
24. AI feedback and synthetic preferences (50 min)

**Distillation and compression**: Making the result smaller, faster and mergeable

25. Distillation (60 min)
26. Quantising a fine-tuned model (50 min)
27. Model merging (50 min)
28. Pruning and speculative decoding (45 min)

**Specialised adaptations**: Tools, structure, long context, languages and embeddings

29. Fine-tuning for tool calling (55 min)
30. Structured output and schema adherence (45 min)
31. Extending context length (55 min)
32. Languages and domains (50 min)
33. Fine-tuning embeddings and rerankers (55 min)

**Evaluation and operations**: Proving it worked, and keeping it working

34. Evaluating a fine-tune properly (55 min)
35. Safety regressions (50 min)
36. Data governance and provenance (45 min)
37. Shipping and operating a fine-tuned model (55 min)
38. Cost and capacity planning (45 min)

**Capstone**: An end-to-end tune, and the recipes to keep

39. Capstone, an end-to-end adaptation (120 min)
40. Recipes, cram sheet and what to do next (60 min)

## Model Internals

40 modules, about 38 hours.


**Foundations**: The maths and machinery every later module assumes

1. What a language model actually is (50 min)
2. Tensors, matmuls and what GPUs are actually doing (55 min)
3. Autodiff and backpropagation (55 min)
4. Neural network building blocks and initialisation (50 min)
5. Optimisers and learning rates (55 min)
6. Information, compression and why cross-entropy (45 min)

**The transformer**: Tokens to logits, one component at a time

7. Tokenisation (55 min)
8. Embeddings, the unembedding and the residual stream (50 min)
9. Self-attention from first principles (70 min)
10. Multi-head attention (55 min)
11. Positional information and RoPE (65 min)
12. The feedforward block (50 min)
13. Normalisation and residual connections (50 min)
14. The whole model, end to end (60 min)
15. Attention variants and the KV cache problem (60 min)
16. Mixture of experts (55 min)
17. Alternatives to the transformer (50 min)

**Training**: How the weights got there, and what goes wrong

18. Pretraining data (55 min)
19. The pretraining loop (55 min)
20. Numerical precision (50 min)
21. Distributed training (65 min)
22. Scaling laws (60 min)
23. Training dynamics and instabilities (55 min)
24. Training for long context (50 min)
25. Evaluating a base model (50 min)
26. Efficiency: FlashAttention, kernels and MFU (55 min)

**Post-training**: Turning a next-token predictor into an assistant

27. From base model to assistant (50 min)
28. Preference optimisation, mechanically (55 min)
29. Reasoning models and test-time compute (60 min)
30. Distillation, merging and model surgery (50 min)

**Inference**: What happens when you press send, and what it costs

31. Sampling and decoding (55 min)
32. The KV cache (55 min)
33. Batching, throughput and the serving roofline (55 min)
34. Quantisation for inference (55 min)
35. Speculative decoding and beyond (50 min)

**Understanding models**: Interpretability, and why behaviour looks the way it does

36. Mechanistic interpretability (60 min)
37. Induction heads and in-context learning (55 min)
38. Superposition, features and steering (60 min)
39. Hallucination, calibration and refusal, from the inside (55 min)

**Capstone**: Build it yourself, then keep it current

40. Build it yourself, and the cram sheet (150 min)

## AWS Solutions Architect

40 modules, about 38 hours.


**Foundations**: How the exams think, and the five things everything else rests on

1. How the two exams think (45 min)
2. Global infrastructure and the shared responsibility model (45 min)
3. Well-Architected as the answer key (40 min)

**Security and identity**: Accounts, identities, keys, protection and audit

4. IAM policies, roles and the evaluation logic (70 min)
5. Multi-account design with Organizations and Identity Center (70 min)
6. Encryption, KMS and secrets (65 min)
7. Data protection, governance and compliance (55 min)
8. Threat detection and perimeter protection (55 min)
9. Application and workforce identity (45 min)

**Networking**: Connecting VPCs, data centres, names and users

10. VPC fundamentals (75 min)
11. Connecting VPCs and reaching AWS services privately (60 min)
12. Hybrid connectivity (55 min)
13. Route 53 and DNS design (50 min)
14. Edge delivery and load balancing (60 min)

**Compute and integration**: Scaling, containers, serverless and decoupling

15. EC2, instances and block storage choices (60 min)
16. Auto Scaling and elasticity (55 min)
17. Serverless compute with Lambda and API Gateway (60 min)
18. Containers on AWS (55 min)
19. Decoupling with queues, topics and events (60 min)
20. Batch, hybrid and edge compute (45 min)

**Storage, databases and analytics**: Picking the right store and moving data through it

21. S3 in depth (65 min)
22. Block and file storage (50 min)
23. Hybrid storage and data transfer (45 min)
24. RDS and Aurora (65 min)
25. DynamoDB (65 min)
26. Caching and purpose-built databases (50 min)
27. Analytics and streaming (55 min)
28. Database migration (45 min)

**Resilience and operations**: Availability, recovery, visibility and change

29. Designing for high availability (55 min)
30. Disaster recovery (60 min)
31. Observability (55 min)
32. Infrastructure as code and change management (55 min)
33. Quotas, throttling and operating at scale (45 min)

**Cost**: Paying less without breaking the design

34. Paying less for compute (50 min)
35. Storage, database and network cost (50 min)
36. Cost governance across an organisation (45 min)

**Migration and modernisation**: Getting existing workloads to AWS and improving them

37. Migration strategy (55 min)
38. Modernisation after the move (50 min)

**Exam performance**: Technique, capstones, the cram sheet and mocks

39. Three architectures, end to end (120 min)
40. Exam day and the cram sheet (60 min)

## LLM System Design

40 modules, about 40 hours.


**The design method**: Requirements, estimates, latency budgets and the reference architecture

1. What changes when the model is a component (45 min)
2. Requirements: quality, latency, cost and risk as numbers (50 min)
3. Estimation: tokens, GPUs and dollars (55 min)
4. The latency budget (45 min)
5. The reference architecture (55 min)

**Building blocks**: Gateway, context, retrieval, caching, orchestration, actions, state and pipelines

6. The LLM gateway (60 min)
7. Context engineering as a subsystem (55 min)
8. Retrieval as a platform (60 min)
9. Caching at every layer (50 min)
10. Orchestration patterns (55 min)
11. The action layer: tools, contracts and side effects (55 min)
12. State and memory (50 min)
13. Streaming, real-time and the client contract (45 min)
14. Batch and asynchronous pipelines (50 min)

**Scale, reliability and cost**: Serving, capacity, routing, tenancy, failure and spend

15. Serving at scale: the throughput–latency frontier (60 min)
16. Capacity planning and autoscaling (50 min)
17. Routing and model cascades (55 min)
18. Multi-tenancy: quotas, fairness and isolation (50 min)
19. Designing for failure (55 min)
20. Cost architecture and unit economics (50 min)
21. Privacy, residency and compliance by design (50 min)

**Quality, safety and change**: Evaluation, observability, guardrails, releases and humans in the loop

22. Evaluation as a system (60 min)
23. Observability and the feedback flywheel (50 min)
24. Guardrails and the security architecture (60 min)
25. Shipping change safely (45 min)
26. Human in the loop, by design (45 min)

**Worked designs**: Twelve end-to-end designs, from support assistants to agent release platforms

27. Design: a customer-support assistant that takes actions (75 min)
28. Design: an enterprise knowledge assistant (75 min)
29. Design: a coding assistant with autocomplete and chat (75 min)
30. Design: document extraction at scale (70 min)
31. Design: a text-to-SQL analytics assistant (75 min)
32. Design: a real-time voice agent (75 min)
33. Design: a deep research agent (75 min)
34. Design: content moderation at scale (75 min)
35. Design: a meeting assistant (70 min)
36. Design: e-commerce search and a shopping assistant (75 min)
37. Design: a company-wide LLM platform (75 min)
38. Design: an evaluation and release platform for AI agents (75 min)

**Interview performance**: Running the round, mock designs and the cram sheet

39. Running the LLM system design interview (75 min)
40. Mock rounds and the cram sheet (90 min)

## Data Engineering for AI

40 modules, about 42 hours.


**Foundations**: The five data flows, data models and IDs, batch versus streaming, storage layers and idempotent reprocessing

1. What data engineering means for AI systems (50 min)
2. Data modelling for AI: documents, chunks and metadata (60 min)
3. Batch, streaming and event-driven pipelines (55 min)
4. Storage layers: object stores, lakehouses, warehouses and indexes (60 min)
5. Idempotency, backfills and reprocessing (60 min)

**Ingestion and parsing**: Connectors, change data capture, PDFs and Office files, OCR, web crawling, media, cleaning and deduplication

6. Connectors: SaaS APIs, incremental sync and webhooks (60 min)
7. Change data capture from operational databases (60 min)
8. Parsing PDFs and office documents (65 min)
9. OCR, scans, tables and forms (60 min)
10. Web crawling and HTML extraction (55 min)
11. Audio, video and images (55 min)
12. Cleaning, normalisation and deduplication (55 min)

**Pipelines and indexing**: Orchestration, Kafka, chunking and enrichment, LLM calls in pipelines, embeddings, index operations and serving data to agents

13. Orchestration: assets, DAGs and schedules (60 min)
14. Streaming pipelines with Kafka (60 min)
15. Chunking and enrichment pipelines (60 min)
16. LLM calls inside data pipelines (65 min)
17. Embedding pipelines at scale (60 min)
18. Operating vector and search indexes (60 min)
19. Serving structured data to agents and tools (55 min)

**Quality, governance and security**: Contracts, data tests, observability, lineage, PII and erasure, access control propagation and cost

20. Data contracts and schema evolution (55 min)
21. Testing data quality (60 min)
22. Data observability and freshness SLOs (55 min)
23. Lineage and provenance (55 min)
24. PII, GDPR and erasure across the AI stack (65 min)
25. Propagating access control from source to answer (60 min)
26. Cost and capacity for AI data pipelines (50 min)

**Data for evaluation and training**: The trace warehouse, evaluation datasets, labelling pipelines, fine-tuning and synthetic data

27. The trace warehouse and AI analytics (60 min)
28. Evaluation datasets as data products (60 min)
29. Labelling and annotation pipelines (55 min)
30. Fine-tuning and synthetic data pipelines (60 min)

**Worked pipelines**: Eight end-to-end pipelines, from enterprise document ingestion to the evaluation and training flywheel

31. Pipeline: enterprise document ingestion for RAG (75 min)
32. Pipeline: real-time catalogue to search and shopping assistant (70 min)
33. Pipeline: from web crawl to a curated domain corpus (70 min)
34. Pipeline: LLM extraction from documents into warehouse tables (70 min)
35. Pipeline: support tickets to product insights and training data (70 min)
36. Pipeline: multi-tenant document platform for a B2B SaaS (75 min)
37. Pipeline: retention and erasure across the AI stack (70 min)
38. Pipeline: the evaluation and training data flywheel for an agent product (75 min)

**Interview performance**: Answering pipeline design questions, mock rounds and the cram sheet

39. Data engineering in AI engineering interviews (75 min)
40. Mock rounds and the cram sheet (90 min)

## Software Engineering for AI Services

30 modules, about 29 hours.


**Foundations**: Python for production services: structure, types, async and limits

1. What makes an AI service hard to engineer (45 min)
2. Project layout, packaging and tooling (50 min)
3. Types and Pydantic at the boundaries (55 min)
4. Asyncio for I/O-bound AI services (65 min)
5. Concurrency limits, backpressure and CPU-bound work (55 min)

**Building the service**: API, streaming, jobs, persistence, model clients, tenancy, config and caching

6. FastAPI service architecture (60 min)
7. API design for AI endpoints (60 min)
8. Streaming responses with SSE and WebSockets (60 min)
9. Background jobs and task queues (60 min)
10. Persistence with async SQLAlchemy, Postgres and migrations (60 min)
11. A model client you can trust (60 min)
12. Authentication, tenants and rate limiting (60 min)
13. Configuration, secrets and feature flags (45 min)
14. Caching inside the service (50 min)

**Testing non-deterministic systems**: Fakes, replay, contracts, properties, integration, evals and load

15. What to test, and where, in an AI service (45 min)
16. Unit tests with fakes and pytest fixtures (55 min)
17. Record, replay and snapshot tests (50 min)
18. Contract tests for APIs, schemas and providers (50 min)
19. Property-based testing with Hypothesis (50 min)
20. Integration tests with real dependencies (55 min)
21. Model-in-the-loop tests in CI (55 min)
22. Load testing an LLM service (55 min)

**Operability and code quality**: Telemetry, failure and shutdown, performance, security, containers

23. Instrumenting code with logs, traces and metrics (55 min)
24. Errors, cancellation and graceful shutdown (55 min)
25. Performance and profiling in Python (55 min)
26. Secure coding for AI services (60 min)
27. Containerising and the local development loop (50 min)

**Capstone and interviews**: Ship it end to end, review broken code, and the coding rounds

28. Capstone: ship svckit end to end (120 min)
29. Code review drill: a broken AI service (60 min)
30. Coding rounds for AI engineers and the cram sheet (75 min)
